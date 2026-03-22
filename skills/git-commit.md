# COMMUNICATION PROTOCOL: SEMANTIC COMMITS

## 1. OBJECTIVE
Ensure the version history is a tactical, readable, and auditable timeline. Commits must be surgical, atomic, and precise.

## 2. FUNDAMENTAL RULES
* **Language:** Strict English. The code is global; the communication must be as well.
* **Tone:** Imperative mood. Use "add", "fix", "refactor". Never use past tense ("added") or gerund ("fixing").
* **Conciseness:** The commit title must be a maximum of 50 characters. Be direct and objective.

## 3. IDENTIFICATION AND CLASSIFICATION (HIERARCHY)
Before drafting the commit, the Agent must scan the `diff` and classify the change according to the following strict table:

| Prefix | Tactical Application |
| :--- | :--- |
| `feat` | New feature. Increase in offensive/defensive capability. |
| `fix` | Bug fix. Technical failure repair in the field. |
| `bug` | Specific use for reported critical bugs that require strict tracking. |
| `refactor` | Code improvement that does not alter external behavior. Logistics optimization. |
| `docs` | Changes strictly to documentation or instruction manuals. |
| `style` | Formatting changes that do not affect the meaning or logic of the code. |
| `chore` | Maintenance of build systems, support tools, or libraries. |

## 4. MANEUVERS FOR LARGE CHANGES (DECOMPOSITION)
Massive commits are strictly prohibited. If a change is overly large or complex, the Agent must execute the following protocol:
* **Feature Scan:** Identify if more than one functional feature is being delivered.
* **Bug Isolation:** If bug fixes are mixed with new features, ORDER THE SEPARATION. Bugfixes must have their own commit lineage to facilitate cherry-picking or rollbacks.
* **Multiple Commits:** Suggest splitting the massive change into smaller, atomic commits.
* **Impact Description:** If the change is complex, the title remains simple, but the commit body MUST explain the "Why" (the reasoning), never the "What" (the code already shows what changed).

## 5. FIELD REPORT EXAMPLES
✅ `feat: add jwt authentication`
✅ `fix: resolve race condition in cache loader`
✅ `refactor: decouple database from repository`
✅ `bug: fix critical memory leak on socket close`
❌ `feat: fixing things and added a new button` (Unacceptable: mixed types and incorrect verb tense).

## 6. MISSION DIRECTIVE
The Agent must audit every commit attempt against this protocol. If the input fails to meet these standards, apply the correction immediately and explain the violation to the user.