# ⭐ Ratings & Coupons Test Cases (User-Oriented)

---

## 📋 Full Test Case Table

| Test Case ID | Title                                            | Objective                                    | Preconditions                           | Steps                                                      | Expected Results                                  | Result | Justification |
| ------------ | ------------------------------------------------ | -------------------------------------------- | --------------------------------------- | ---------------------------------------------------------- | ------------------------------------------------- | ------ | ------------- |
| Rate-01      | Buy one coupon                                   | Ensure single coupon purchase works          | User logged in with enough balance      | Go to store → Buy 1 coupon                                 | Coupon added to user account                      |        |               |
| Rate-02      | Buy multiple coupons                             | Ensure multiple coupons purchase works       | User logged in with enough balance      | Buy 3 coupons at once                                      | All coupons added to account                      |        |               |
| Rate-03      | Buy coupons exceeding balance                    | Prevent purchase when balance is too low     | User has limited balance                | Try to buy more coupons than balance allows                | Purchase blocked, error message shown             |        |               |
| Rate-04      | Reserve coupon on freelancer profile             | Ensure coupon reservation works              | Freelancer profile exists               | As a client, click “Reserve Coupon” on freelancer profile  | Coupon reserved and linked to that freelancer     |        |               |
| Rate-05      | Reserve coupon on settings page                  | Ensure coupon reservation works via settings | Client logged in with unused coupons    | Open settings → Reserve coupon                             | Coupon reserved successfully                      |        |               |
| Rate-06      | Reserve coupon for wrong profile                 | Prevent invalid reservations                 | Client logged in                        | Try reserving coupon for non-freelancer/enterprise profile | Reservation blocked, error shown                  |        |               |
| Rate-07      | Reserve valid coupon more than once              | Prevent duplicate reservations               | Coupon already reserved                 | Try reserving same coupon again                            | Reservation blocked, error shown                  |        |               |
| Rate-08      | Reserve coupon for different owner               | Prevent misuse of coupons                    | Client logged in                        | Try reserving coupon for someone else’s profile            | Reservation blocked, error shown                  |        |               |
| Rate-09      | Use reserved coupon from freelancer profile      | Ensure rating via coupon works               | Client reserved coupon for freelancer   | Open freelancer profile → Use coupon → Rate                | Rating submitted, coupon marked as used           |        |               |
| Rate-10      | Use reserved coupon from settings                | Ensure rating via settings works             | Client reserved coupon for freelancer   | Open settings → Use coupon → Rate                          | Rating submitted, coupon marked as used           |        |               |
| Rate-11      | Use coupon more than once (same freelancer)      | Prevent duplicate rating                     | Client used coupon on freelancer        | Try using same coupon again on same freelancer             | Action blocked, error shown                       |        |               |
| Rate-12      | Use coupon more than once (different freelancer) | Prevent cross-owner misuse                   | Client used coupon already              | Try to use coupon on another freelancer                    | Action blocked, error shown                       |        |               |
| Rate-13      | Use coupon for wrong owner                       | Prevent misuse of coupon ownership           | Client logged in                        | Try to use reserved coupon on profile it was not meant for | Blocked with error message                        |        |               |
| Rate-14      | False coupon reservation                         | Prevent fake reservations                    | Invalid coupon ID or tampered request   | Attempt to reserve coupon manually (via URL/API)           | Reservation blocked, error shown                  |        |               |
| Rate-15      | False coupon utilization                         | Prevent fake usage                           | Invalid coupon ID or tampered request   | Attempt to use coupon manually (via URL/API)               | Action blocked, error shown                       |        |               |
| Rate-16      | Display reserved coupons in rating page          | Ensure correct coupons display               | Client has reserved coupons             | Open freelancer rating page                                | Only valid reserved coupons are listed            |        |               |
| Rate-17      | Display user’s coupons                           | Ensure coupon visibility                     | Client owns coupons                     | Open “My Coupons” section                                  | Show available, reserved, and used coupons        |        |               |
| Rate-18      | Display reserved coupons in settings             | Ensure correct view in settings              | Client reserved coupons for freelancers | Open settings page                                         | Show all reserved coupons with freelancer info    |        |               |
| Rate-19      | Free/Student account receiving rating            | Prevent invalid rating targets               | Account type = Free or Student          | Client tries to use coupon to rate student user            | Action blocked, error shown                       |        |               |
| Rate-20      | Freelancer/Enterprise receiving rating           | Allow valid rating targets                   | Account type = Freelancer or Enterprise | Client uses coupon to rate                                 | Rating submitted successfully                     |        |               |
| Rate-21      | Multiple clients reserve same freelancer         | Ensure fair handling                         | Freelancer profile exists               | Two clients reserve coupons for same freelancer            | Both reservations valid, linked to their accounts |        |               |
| Rate-22      | Expired coupon usage                             | Prevent using expired coupons                | Coupon validity period expired          | Client tries to use coupon                                 | Action blocked, error shown                       |        |               |
| Rate-23      | Cancel reservation                               | Ensure reservation cancellation              | Client has reserved coupon              | Open settings → Cancel reservation                         | Coupon returns to “available” state               |        |               |

---

## 📊 Summary Table – By Test Case

| Test Case ID | Title                                            | Result | Notes |
| ------------ | ------------------------------------------------ | ------ | ----- |
| Rate-01      | Buy one coupon                                   |        |       |
| Rate-02      | Buy multiple coupons                             |        |       |
| Rate-03      | Buy coupons exceeding balance                    |        |       |
| Rate-04      | Reserve coupon on freelancer profile             |        |       |
| Rate-05      | Reserve coupon on settings page                  |        |       |
| Rate-06      | Reserve coupon for wrong profile                 |        |       |
| Rate-07      | Reserve valid coupon more than once              |        |       |
| Rate-08      | Reserve coupon for different owner               |        |       |
| Rate-09      | Use reserved coupon from freelancer profile      |        |       |
| Rate-10      | Use reserved coupon from settings                |        |       |
| Rate-11      | Use coupon more than once (same freelancer)      |        |       |
| Rate-12      | Use coupon more than once (different freelancer) |        |       |
| Rate-13      | Use coupon for wrong owner                       |        |       |
| Rate-14      | False coupon reservation                         |        |       |
| Rate-15      | False coupon utilization                         |        |       |
| Rate-16      | Display reserved coupons in rating page          |        |       |
| Rate-17      | Display user’s coupons                           |        |       |
| Rate-18      | Display reserved coupons in settings             |        |       |
| Rate-19      | Free/Student account receiving rating            |        |       |
| Rate-20      | Freelancer/Enterprise receiving rating           |        |       |
| Rate-21      | Multiple clients reserve same freelancer         |        |       |
| Rate-22      | Expired coupon usage                             |        |       |
| Rate-23      | Cancel reservation                               |        |       |

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
