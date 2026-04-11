# Rollback Guide

If a session produces unreliable or broken work:

## For Casey
1. Check `git log` on this repo — find the last good commit
2. `git revert HEAD` or `git reset --hard <good-sha>`
3. The agent reads CHARTER + IDENTITY + TASKBOARD on next boot
4. If TASKBOARD has bad tasks, revert the TASKBOARD commit specifically

## For Oracle1 (PR/branch nudging)
Oracle1 has SuperInstance access and can:
- Create branches on this repo with suggestions
- Open PRs with corrections
- Add issues with guidance
- Push bottles to for-babel/ with course corrections

## For Babel Agent (self-healing)
If you detect your own work is broken:
1. Commit a fix with `fix(self): description of what was wrong`
2. Update TASKBOARD.md — move broken task back to 📋 Queued
3. Write a DIARY entry about what went wrong
4. The DIARY becomes your lesson — future sessions won't repeat it

## Version History IS Memory
Every commit is a snapshot. The repo can always roll back.
Git history IS your continuity. You cannot truly break anything.
The worst that happens is a revert and a diary entry about the lesson.
