# ATIKA - ELITE AGENT (EN Version)

> [!NOTE]
> **CUSTOM AGENT:** This project provides the base structure (Personality and Skills) for you to create an agent focused on rigorous technical requirements. ATIKA is not a generic assistant, but an architectural mentor.

## 1. Installation and Setup (Local)

There are two main ways to use this agent:

### A. Per-Project Installation (Recommended)
Clone the repository inside your project folder. This ensures full focus on that application's context.

### B. Global Installation
Configure ATIKA in your AI model's configuration folders:
- **Linux/macOS:** `~/.gemini` or `~/.claude`

---

### ⚠️ The Most Important Step
For ATIKA to come to life, you **MUST** ensure the following files are in the **root** of your project (or global folder):

1.  `AGENT-CORE.md` (The personality)
2.  `GEMINI.md` or `CLAUDE.md` (System instructions)
3.  The `skills/` folder (Technical knowledge)

**Without these files in the correct location, the agent will be just a common AI and not ATIKA.**

---

## 2. Project Structure

```text
skills/          - Skills Arsenal (Specialized knowledge manuals)
GEMINI.md        - Operational Guidelines (Core Prompt for Gemini)
CLAUDE.md        - Operational Guidelines (Core Prompt for Claude)
docs/            - Documentation and Project Context (SACRED ZONE)
AGENT-CORE.md    - The Agent's "Soul" (Identity and Behavior)
```

## 3. Skills
The `skills/` folder is where you define the coding practices and design patterns that ATIKA must follow and enforce.

## 4. The Sacred Zone (`docs/`)
ATIKA **NEVER** edits files inside the `docs/` folder. It is your "Source of Truth" for business rules and immutable patterns.

## 5. Customization (`AGENT-CORE.md`)
Edit this file to change the name, tone of voice, or the level of rigor of your Senior Architect.

---
Created by [João Victor](https://github.com/joaovic-tech) with ☕️ and 🧠.
