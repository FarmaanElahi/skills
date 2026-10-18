---
name: link
description: Link one skill from this repository's skills folder into the project agent skills directory.
---

# Link a skill

Use this skill to install or update one skill at a time from `skills/` into `.agents/skills/`.

Given a skill name, use `skills/<name>` as the source and `.agents/skills/<name>` as the destination. Create the destination parent if needed. If the destination is already a symlink to that source, leave it unchanged. If another file or directory already exists at the destination, stop and report the conflict. Never link the entire `skills/` folder.

For example, from the repository root:

```sh
ln -s ../../skills/unslop .agents/skills/unslop
```
