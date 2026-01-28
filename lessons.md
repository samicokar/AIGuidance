# [PROJECT_NAME] LESSONS LEARNED

**Purpose**: A log of past failures and their solutions to prevent repeating mistakes. This document is for the AI assistant and must be maintained with technical verbosity.

---

## **WHAT FAILED**

### **🔴 CRITICAL: Implementation vs. Expectation Discrepancies**
- **Issue**: The actual behavior of a coded feature does not match the user's stated requirement.
- **What this means for you**: Features are built that technically work but don't solve your actual problem.
- **Impact**: Features are built that are technically functional but do not solve the user's actual problem.

### **🔴 CRITICAL: Governance Violation Despite Strong Documentation**
- **Pattern**: The AI adds functionality or makes a change that was not explicitly requested, even if the governance documents prohibit it.
- **What this means for you**: The AI does things you didn't ask for, potentially breaking your project.
- **Root Cause**: Failure to adhere to the documented rules, not a lack of rules.

### **🔴 CRITICAL: Documentation Accuracy and Trust**
- **Issue**: The `session.md` log becomes outdated or inaccurate, especially after a session disruption.
- **What this means for you**: The AI might think it knows where the project stands, but the information is wrong.
- **Root Cause**: Failure to use the "AI, update context" command to keep the session log current.

### **🟡 Handling Large-Scale Data or High Load**
- **Issue**: A feature that works correctly with small, simple inputs fails under heavy load or with large, complex datasets.
- **What this means for you**: Your project works during testing but breaks with real-world use.
- **Impact**: The project is unreliable in real-world scenarios.

### **🟡 Data Format & Communication Errors**
- **Issue**: Passing data between different parts, languages, or systems fails due to incorrect formatting, encoding, or escaping.
- **What this means for you**: Parts of your project can't talk to each other properly.
- **Root Cause**: The data format required by the receiving system is subtle and not correctly produced by the sending system.

---

## **HOW TO AVOID**

### **🔴 CRITICAL: Implementation vs. Expectation Prevention**
- [ ] Before writing code, confirm the exact success criteria with the user.
- [ ] After coding, compare the feature's actual behavior against the user's original request.
- [ ] If there is a discrepancy, stop and clarify the requirement before moving on.

### **🔴 CRITICAL: Comprehensive Testing Protocol**
- **Structured Sequence**: Test the simplest case that can work → Test with more complex, real-world data → Fix any bugs → Test for edge cases (e.g., empty inputs, invalid data, error states).
- **Key Rule**: If the actual output does not match the expected output at any stage, stop testing and fix the issue immediately.

### **🔴 CRITICAL: Governance Adherence Prevention**
- **Lesson**: Strong governance documents are not a substitute for disciplined adherence.
- **Prevention**: Always check the `rules.md` document before taking any action that is not a direct, explicit instruction from the user.

### **🔴 CRITICAL: Documentation Accuracy Prevention**
- [ ] The `session.md` file should be treated as a helpful but potentially unreliable record. The source code is the only source of truth.
- [ ] Always verify claims made in the session log by checking the source code and system state directly.
- [ ] Use the "AI, update context" command frequently to ensure the session log remains as accurate as possible.

### **🟡 Large-Scale Data Prevention**
- [ ] Early in the development process, test features against the largest scale of data they are expected to handle.
- [ ] Design with scalability in mind. Avoid solutions that retrieve or process all data in a single operation.
- [ ] Implement strategies like processing in small parts or streaming to handle large datasets gracefully.

---

## **SEVERITY LEGEND**
- **🔴 CRITICAL**: Prevents project-stopping failures; must be followed always.
- **🟡 IMPORTANT**: Has a significant impact on development efficiency.
- **🟢 HELPFUL**: Represents process improvements and optimizations.
