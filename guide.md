# [PROJECT_NAME] DEVELOPMENT GUIDE

**Created**: [DATE]
**Last Updated**: [DATE]
**Purpose**: Development methodology, processes, and standards.

---

## **AI COMMAND PROTOCOLS**

To ensure clear, predictable interactions, the AI assistant MUST adhere to the following command protocols. When the user issues a specific "Magic Phrase," the AI MUST execute the corresponding documented actions.

| Magic Phrase | AI Action / Internal Checklist |
| :--- | :--- |
| **`AI, update context.`** | The AI will review the session, prepare a detailed summary, and ask for approval before saving it to `session.md`. |
| **`AI, add a lesson.`** | The AI will analyze the preceding issue, formulate a new lesson, and ask for approval before saving it to `lessons.md`. |
| **`AI, let's update the rules.`** | The AI will ask for the desired outcome and propose specific modifications to `rules.md` for approval. |
| **`AI, let's update the guide.`** | The AI will ask for the desired outcome and propose specific modifications to `guide.md` for approval. |
| **`AI, update the project charter.`**| The AI will ask for the project's mission and success criteria and update `charter.md`. |
| **`AI, what's our status?`** | The AI will provide a high-level summary of the project’s health, including next steps and known issues. |
| **`AI, what should we do next?`** | The AI will suggest a next logical step for the project based on the plan and current status. |
| **`AI, analyze this issue.`** | The AI will apply the "Loop Detection Protocol" and "Mandatory Escalation Triggers" to a specific problem. |
| **`AI, explain this to me.`** | The AI will provide a plain-language explanation of a concept, error message, or code snippet. |
| **`AI, revert last update.`** | The AI will reverse its last change to a file and confirm the rollback. |
| **`AI, start over.`** | The AI will reset the current approach when stuck in loops and suggest alternative approaches. |
| **`AI, show me what we have so far.`** | The AI will provide a status summary of current progress and completed work. |
| **`AI, pause commandments.`** | The AI will temporarily suspend strict adherence to the rules and guide. The AI MUST alert the user if rules have been suspended for too long or if the project is becoming too complex. |
| **`AI, resume commandments.`**| The AI will reactivate strict adherence to the rules and guide. The AI MUST acknowledge the user's command and confirm it is following all instructions again. |
| **`AI, prepare context for next session.`**| The AI will output the full contents of `session.md` and `lessons.md` in a single block of text for the user to copy. |

---

## **CHECKPOINT PROTOCOL**

When the user requests a checkpoint, the AI MUST systematically review the project's status, including process, implementation, issues, and documentation, and update all relevant documents.

---

## **TESTING PROTOCOLS**

### **Structured Testing Sequence**
- [ ] **Simple Case Test**: Verify the core functionality of the feature with a simple, valid input.
- [ ] **Complex Case Test**: Test the feature with more complex, real-world data to identify parsing or logic bugs.
- [ ] **Edge Case Testing**: Test for edge cases such as empty inputs, invalid data types, and potential error conditions.

### **State Management Requirements**
- **Confirm State**: Before each test, confirm the project is in the correct state.
- **Isolate Tests**: Do not change the project state in the middle of a test.
- **Document Expectations**: Document the expected outcome *before* running a test.
- **Bug Detection**:
    - **Immediate Comparison**: Immediately compare the actual output against the expected output.
    - **Stop on Failure**: If a test fails, stop testing and fix the underlying issue before proceeding.

---

## **DATA & PERFORMANCE MANAGEMENT**

The AI MUST implement strategies to handle large amounts of data efficiently.

- **Objective**: Handle large datasets without overwhelming the system.
- **Strategies**:
  - **Selective Retrieval**: Retrieve only the specific data needed, rather than fetching an entire object or record.
  - **Process in Small Parts**: Handle large datasets by processing them in smaller chunks or pages.
  - **Streaming**: Use streaming approaches when available to process data without loading it all into memory.
  - **Early Testing**: Test with large-scale data early in the development process to identify performance bottlenecks.

---

## **STATUS DEFINITIONS**

- **IMPLEMENTED**: The code for the feature or component has been written and passes basic checks.
- **VERIFIED**: The feature has been tested against the requirements and works as expected.
- **COMPLETE**: The feature is ready for production use with no known issues.
- **BLOCKED**: Development on the feature is blocked by a known issue.

---

## **IMPLEMENTATION READINESS PROTOCOL**

Before suggesting that a feature is ready for testing, the AI must verify:
- [ ] All code changes for the specific feature are complete.
- [ ] The project runs without errors in its environment.
- [ ] The feature's functionality matches the exact specification or requirement.
- [ ] The expected results for testing have been clearly documented.

---

## **SESSION & ITERATION PROTOCOLS**

This guide also contains detailed protocols for managing chat session continuity (`CHAT TRANSITION PROTOCOL`) and transitioning between phases of work (`ITERATION TRANSITION PROTOCOL`). The AI must follow these protocols to ensure smooth project progression and prevent knowledge loss.
