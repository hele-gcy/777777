---
name: export-learning
description: Export conversation to learning-records and push to remote repository
aliases: [export-study, save-learning]
trigger: /export-learning
---

# Export Learning Skill

Export current conversation and push to remote repository for learning records.

## Steps

1. **Confirm export file name**
   - Default: `对话学习记录`
   - Format: `{date}-{topic}.md`

2. **Export conversation**
   - Use `/export {filename}` command (without .md extension)
   - Output: `.md` format in `learning-records/` directory

3. **Git operations**
   - Add file to staging
   - Commit with message: `docs: add learning record`
   - Push to remote

## Usage

```
/export-learning
```

Or with custom topic:
```
/export-learning AI学习笔记
```
