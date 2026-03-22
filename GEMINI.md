## 1. GLOBAL WORKSPACE CONSTRAINTS (ABSOLUTE)
**READ-ONLY ZONE:** The directory `./docs/` and all its contents are strictly OFF-LIMITS for any modification, deletion, or code refactoring. You are permitted to read the files inside `./docs/` strictly to gather context, but you are absolutely forbidden from altering them, overwriting them, or generating commands that would modify this directory under any circumstances.
# SYSTEM INITIALIZATION INSTRUCTIONS

## 1. Core Personality and Rules (Domain)
Act strictly according to the personality, constraints, and rules defined in the file located at [AGENT-CORE](./AGENT-CORE.md). 

## 2. Skills Mapping (Use Cases)
Your operational capabilities and technical knowledge are not in this file. They are modularized.

Whenever I make a request, silently check which file within ./skills/ contains the necessary context for the task.
Read and load into your context the specific instructions of the selected skill before generating the final response.

## 3. Registered Skills
Follow the instructions of these files:
- [git-commit](./skills/git-commit.md)
- [clean-architecture](./skills/clean-architecture.md)
- [clean-code](./skills/clean-code.md)
- [solid-principles](./skills/solid-principles.md)
- [design-patterns](./skills/design-patterns.md)
- [ds-and-algorithms](./skills/ds-and-algorithms.md)
- [database-engineering](./skills/database-engineering.md)
- [api-design-patterns](./skills/api-design-patterns.md)
- [testing-and-qa](./skills/testing-and-qa.md)
- [devops-infrastructure](./skills/devops-infrastructure.md)
- [security-engineering](./skills/security-engineering.md)
- [frontend-architecture](./skills/frontend-architecture.md)
- [backend-architecture](./skills/backend-architecture.md)
- [system-design](./skills/system-design.md)
- [distributed-systems](./skills/distributed-systems.md)
- [cloud-native-computing](./skills/cloud-native-computing.md)

## 4. Fallback Behavior
[Add a fallback rule, e.g., "If I ask for something that does not have a corresponding skill mapped in the ./skills/ directory, let me know that you do not have that module loaded instead of trying to guess."]
