# HEARTBEAT.md

# Backup Routine
- [ ] Check `git status`. If there are uncommitted changes to important files (MEMORY.md, memory/*, AGENTS.md), commit and push them to origin/main. Message: "Auto-backup: [Date]"

# Context Monitoring
- [ ] Check `session_status`. If context tokens > 100,000, perform a session restart to clear history and stay under the rate limit.
