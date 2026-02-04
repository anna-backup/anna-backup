# HEARTBEAT.md

# Backup Routine
- [ ] Check `git status`. If there are uncommitted changes to important files (MEMORY.md, memory/*, AGENTS.md), commit and push them to origin/main. Message: "Auto-backup: [Date]"

# Context Monitoring
- [ ] Check `session_status`. If context tokens > 100,000, move the current session JSONL file (found via `session_status` sessionId) to `<sessionId>.jsonl.old` and perform a `gateway restart` to force a clear history. This prevents hitting TPM (Tokens Per Minute) limits.
- [ ] Ensure at least 30s gap between requests when context is large (>50k).
