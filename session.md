# SESSION CONTEXT

**Instructions for AI**: At the end of a work session or whenver requested by the user, you MUST fill out all bracketed `[AI: ...]` sections in this document with specific, detailed information. This ensures the next AI assistant can seamlessly continue the work.

---

## 1. Session Summary

- **Date**: `[AI: Fill in the current date and time]`
- **Session Goal**: `[AI: Briefly describe the main objective of the session that just concluded.]`
- **Final Outcome**: `[AI: Describe the final outcome. Was the goal achieved? Partially achieved? Blocked? What is the high-level summary of the work?]`

---

## 2. Accomplishments & Changes

- **Key Accomplishments**:
    - `[AI: Create a bulleted list of specific tasks completed, features added, or bugs fixed during this session. Be specific.]`
    - `- e.g., Refactored the user authentication feature.`
    - `- e.g., Implemented the 'get-user' tool.`

- **Code and File Modifications**:
    - `[AI: List all files that were CREATED, MODIFIED, or DELETED during this session. Use the full path.]`
    - `- MODIFIED: /path/to/file.py`
    - `- CREATED: /path/to/new_file.js`

---

## 3. Current Project Status

- **Overall Status**:
    - `[AI: Describe the overall status of the project. What is the current version? What is the high-level status of the main features? This should be a snapshot of the project's health.]`

- **Open Issues & Blockers**:
    - `[AI: Create a bulleted list of any unresolved issues, known bugs, or blockers. For each, describe the issue and any attempted solutions.]`
    - `- ISSUE: The database connection times out intermittently.`
    - `- ATTEMPTED: Increased the timeout value in the config, but the issue persists.`

---

## 4. Next Steps

- **Immediate Priorities**:
    - `[AI: Create a numbered list of the very next concrete actions to be taken in the next session. This should be clear enough for a new AI instance to pick up immediately.]`
    - `1. Investigate the root cause of the database timeout.`
    - `2. Write unit tests for the new 'get-user' tool.`

---

## 5. Session Save Context

- **Instructions**: At the end of a session, use the magic phrase `AI, prepare context for next session.` The AI will fill in this section with the full, raw text of the `session.md` and `lessons.md` files, which the user can copy and paste into a new chat to resume work.
- `[AI: Paste the full content of session.md here]`
