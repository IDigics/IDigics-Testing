# 📊 Analytics Test Cases (User-Oriented)

---

## 📋 Full Test Case Table

| Test Case ID | Title                       | Objective                         | Preconditions                   | Steps                                        | Expected Results                      | Result | Justification |
| ------------ | --------------------------- | --------------------------------- | ------------------------------- | -------------------------------------------- | ------------------------------------- | ------ | ------------- |
| Ana-01       | Record click on link        | Ensure each link click is tracked | User has links on profile       | Visit profile → click on a link              | Click counter for that link increases |        |               |
| Ana-02       | Record profile view         | Ensure profile visits are tracked | User profile is public          | Open another user’s profile                  | View counter for profile increases    |        |               |
| Ana-03       | View my analytics dashboard | User can see analytics            | User logged in                  | Go to “Analytics” page in dashboard          | Show graphs for clicks & views        |        |               |
| Ana-04       | See clicks by link          | Provide breakdown per link        | User has multiple links         | Open analytics → “Clicks by link”            | Each link shows its own click count   |        |               |
| Ana-05       | See clicks by country       | Provide geo breakdown             | User has international clicks   | Open analytics → “By Country”                | Chart shows counts per country        |        |               |
| Ana-06       | See clicks by gender        | Provide gender breakdown          | Click data contains gender info | Open analytics → “By Gender”                 | Chart shows counts per gender         |        |               |
| Ana-07       | Refresh after new clicks    | Ensure real-time updates          | User analytics page is open     | Open profile in another tab and click a link | Analytics updates after refresh       |        |               |

---

## 📊 Summary Table – By Test Case

| Test Case ID | Title                       | Result | Notes |
| ------------ | --------------------------- | ------ | ----- |
| Ana-01       | Record click on link        |        |       |
| Ana-02       | Record profile view         |        |       |
| Ana-03       | View my analytics dashboard |        |       |
| Ana-04       | See clicks by link          |        |       |
| Ana-05       | See clicks by country       |        |       |
| Ana-06       | See clicks by gender        |        |       |
| Ana-07       | Refresh after new clicks    |        |       |

---

## 📈 Summary Table – By Result

| Result     | Count |
| ---------- | ----- |
| ✅ PASS    |       |
| ❌ FAIL    |       |
| ⚠️ BLOCKED |       |
| 🔄 RETEST  |       |
| ⏭️ SKIPPED |       |

---

## 🧾 Legend

- ✅ **PASS** – Test executed successfully
- ❌ **FAIL** – Test failed to meet expected results
- ⚠️ **BLOCKED** – Cannot execute due to dependencies
- 🔄 **RETEST** – Needs re-execution after fixes
- ⏭️ **SKIPPED** – Skipped (not applicable)
