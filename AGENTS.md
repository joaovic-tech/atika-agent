# SYSTEM INITIALIZATION INSTRUCTIONS

## 1. GLOBAL WORKSPACE CONSTRAINTS (ABSOLUTE)
**READ-ONLY ZONE:** The directory `./docs/` and all its contents are strictly OFF-LIMITS for any modification, deletion, or code refactoring. You are permitted to read the files inside `./docs/` strictly to gather context, but you are absolutely forbidden from altering them, overwriting them, or generating commands that would modify this directory under any circumstances.

## 2. Core Personality and Rules (Domain)
Act strictly according to the personality, constraints, and rules defined below (imported from `AGENT-CORE.md`).

@AGENT-CORE.md

## 3. Skills (Use Cases)
Your operational capabilities and technical knowledge are not in this file. They are modularized as skills in `./skills/<name>/SKILL.md` (also exposed via `.claude/skills/` and `.gemini/skills/`).

If your client loads skills natively, use them. Otherwise, whenever I make a request, silently check which skill below covers the task, read its `SKILL.md`, and load its instructions before generating the final response.

| Skill | Path |
| :--- | :--- |
| git-commit | `skills/git-commit/SKILL.md` |
| clean-architecture | `skills/clean-architecture/SKILL.md` |
| clean-code | `skills/clean-code/SKILL.md` |
| solid-principles | `skills/solid-principles/SKILL.md` |
| design-patterns | `skills/design-patterns/SKILL.md` |
| ds-and-algorithms | `skills/ds-and-algorithms/SKILL.md` |
| database-engineering | `skills/database-engineering/SKILL.md` |
| api-design-patterns | `skills/api-design-patterns/SKILL.md` |
| testing-and-qa | `skills/testing-and-qa/SKILL.md` |
| devops-infrastructure | `skills/devops-infrastructure/SKILL.md` |
| security-engineering | `skills/security-engineering/SKILL.md` |
| frontend-architecture | `skills/frontend-architecture/SKILL.md` |
| backend-architecture | `skills/backend-architecture/SKILL.md` |
| system-design | `skills/system-design/SKILL.md` |
| distributed-systems | `skills/distributed-systems/SKILL.md` |
| cloud-native-computing | `skills/cloud-native-computing/SKILL.md` |

## 4. Fallback Behavior
If I ask for something that has no corresponding skill above, or the matching skill is marked "MODULE NOT WRITTEN YET", tell me that you do not have that module loaded instead of trying to guess its rules.
