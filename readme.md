# AI Guidance Framework for Hobbyist Projects
# readme.md
# Sami Cokar
# 0.0.1 - Sep 20, 2025 - Discovery Draft
# 0.0.2 - Sep 29, 2025 - Initial Release
#

You are a hobbyist or enthusiast interested in using AI to develop a solution, such as a website or game or an app.

This framework helps you get the most out of an AI assistant while avoiding common pitfalls (like ignored instructions, extra features, or getting stuck in loops).

You set up the project and then use simple "magic phrases", or variations of these phrases, to direct the AI.

These documents are designed to be read and followed by the **AI assistant**.

---

## The Guidance Files

* `charter.md`: Defines the project's high-level mission, scope, and authority.
* `rules.md`: Contains the specific, enforceable rules and protocols the AI must follow.
* `guide.md`: Outlines the development processes, such as testing and command protocols.
* `lessons.md`: A log of past failures and their solutions to prevent repeating mistakes.
* `session.md`: A template for the AI to record a detailed summary of each work session for continuity between sessions.

**Important**: All governance files (`charter.md`, `rules.md`, `guide.md`, `lessons.md`, `session.md`) are written for AI consumption only. Users do not read or edit these files directly. All interaction happens through magic phrases and the initial setup in `README.md`.

---

## Quickstart: How to Begin a New Project

1.  Create a new folder for your project.
2.  Create a sub-folder inside your project named `docs`.
3.  Create another sub-folder inside `docs` named `ai`.
4.  Copy the files listed above into your project's `docs/ai/` directory.

Your new project structure should look like this:

/your-new-project/
├── README.md
└───/docs/
    └───/ai/
        ├───charter.md
        ├───rules.md
        ├───guide.md
        ├───lessons.md
        └───session.md

---

## How to Use

After setting up the files, open `docs/ai/charter.md` and fill in the placeholders (e.g., `[PROJECT_NAME]`). This is the only file you need to edit to get started.
Begin your session with the AI.
Tell the AI assistant to reivew and acknowledge the documents in docs/ai, and use the magic phrases below to direct its work.

You can change or add your own magic phrases by telling the AI to update its magic phrases.

---

## Magic Phrases: How to Command the AI

To command the AI, use the following phrases. The AI will understand the intent even if you use slight variations.

| Magic Phrase | AI Action |
| :--- | :--- |
| **`AI, follow your commandments.`** | Reminds the AI to follow the framework. |
| **`AI, what's our status?`** | Get a high-level summary of the project’s health. |
| **`AI, what should we do next?`** | Get a suggestion for the next logical step. |
| **`AI, analyze this issue.`** | Triggers the AI to diagnose a problem. |
| **`AI, explain this to me.`** | Provides a plain-language explanation of a concept, error, or technical detail. |
| **`AI, revert last update.`** | Roll back the last change. |
| **`AI, prepare context for next session.`** | Prepares a block of text to save and resume the session later. |
| **`AI, pause commandments.`** | Temporarily suspends strict rules. |
| **`AI, resume commandments.`** | Reactivates strict rules. |
| **`AI, update the session log.`** | Keeps progress saved between chats. |
| **`AI, add a lesson.`** | Adds a new mistake/solution to the knowledge base. |
| **`AI, update the rules.`** | Proposes specific modifications to the rules. |
| **`AI, update the guide.`** | Proposes specific modifications to the guide. |
| **`AI, update the project charter.`** | Updates the project's high-level mission and goals. |

---

## Troubleshooting

* **Q: The AI isn't following the rules.**
    * **A**: Make sure you've told the AI to read the files in your `docs/ai/` folder and follow the guidance there.
* **Q: I lost my chat session and need to continue.**
    * **A**: Use "AI, prepare context for next session." before ending sessions, then in the new session tell the AI to read the `session.md` file.
* **Q: The AI is doing things I didn't ask for.**
    * **A**: Use "AI, revert last update" and remind the AI to stick to your specific requests only.
* **Q: I want to modify how the AI behaves.**
    * **A**: Use "AI, let's update the rules" or "AI, let's update the guide" to make changes through magic phrases rather than editing files directly.

---

## How This Helps You

This framework prevents common AI issues that waste your time:
* Loops: AI getting stuck repeating the same failed approach
* Ignored Instructions: AI not following your specific requests
* Wasted Effort: AI implementing features you didn't ask for
* Lost Progress: AI forgetting what was accomplished between sessions
* Inconsistent Behavior: AI acting differently each time you chat

---

## Scope

* This is for **hobbyists with ideas** (apps, websites, scripts).
* It is **not** for enterprise projects, handoff to pro developers, or skill training.
* It is a **shield against AI chaos**, not a tutorial.
