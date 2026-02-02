# HEARTBEAT.md

# Backup Routine
- [ ] Check `git status`. If there are uncommitted changes to important files (MEMORY.md, memory/*, AGENTS.md), commit and push them to origin/main. Message: "Auto-backup: [Date]"

# Context Monitoring
- [ ] Check `session_status`. If context tokens > 80,000, notify Martin and suggest a gateway restart to stay under the 100k/min rate limit.
