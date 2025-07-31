> This template is designed to help you create clear, organized, and modern test documentation for any software system or feature, facilitating consistent reporting and easier collaboration.

---

# 🧪 {featureTitle} Test Cases

---

## 📋 Full Test Case Table

| Test Case ID | Title              | Objective                         | Preconditions               | Steps                         | Expected Results              | Result | Justification |
|--------------|--------------------|---------------------------------|-----------------------------|-------------------------------|------------------------------|--------|----------------|
| TC-01        | Example Test Case 1 | Write objective here             | Write preconditions here     | Write steps here              | Write expected results here  |        |                |
| TC-02        | Example Test Case 2 | Write objective here             | Write preconditions here     | Write steps here              | Write expected results here  |        |                |
| TC-03        |                    |                                 |                             |                               |                              |        |                |
| ...          |                    |                                 |                             |                               |                              |        |                |

---

**Notes:**  
- **Justification** is **optional** when the test result is **✅ PASS**.  
- **Justification** is **required** for all other results (❌ FAIL, ⚠️ BLOCKED, 🔄 RETEST, ⏭️ SKIP) to provide clear reasoning.  

---

## 📊 Summary Table – By Test Case

| Test Case ID | Title             | Result | Notes |
|--------------|-------------------|--------|-------|
| TC-01        | Example Test Case 1|        |       |
| TC-02        | Example Test Case 2|        |       |
| TC-03        |                   |        |       |
| ...          |                   |        |       |

---

**Notes:**  
- Filling out the **Notes** column is **important** for providing feedback and suggesting improvements.  
- Please use it to explain any issues, observations, or remarks during testing.  

---

## 📈 Summary Table – By Result

| Result     | Count |
|------------|-------|
| ✅ PASS     |       |
| ❌ FAIL     |       |
| ⚠️ BLOCKED |       |
| 🔄 RETEST  |       |
| ⏭️ SKIP    |       |

---

**Notes:**  
- Update the **Count** column based on the total number of test cases with each result after testing is completed.  

---

## 🗂️ Legend

- ✅ **PASS** – Test executed successfully  
- ❌ **FAIL** – Test failed to meet expected results  
- ⚠️ **BLOCKED** – Cannot execute due to dependencies  
- 🔄 **RETEST** – Needs re-execution after fixes  
- ⏭️ **SKIP** – Skipped (not applicable)
