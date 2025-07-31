# ✅ Authentication Test Cases

---

## 📋 Full Test Case Table

| Test Case ID | Title | Objective | Preconditions | Steps | Expected Results | Result | Justification |
|--------------|-------|-----------|----------------|-------|------------------|--------|----------------|
| Auth-01 | Access pages unauthenticated | Block unauthenticated access | User not logged in | Try /dashboard, settings, admin | Redirect to login, no data shown |  |  |
| Auth-02 | Sign up with used email | Prevent duplicate email registration | Email exists | Submit existing email | Block form, show error |  |  |
| Auth-03 | Sign up with used username | Prevent duplicate usernames | Username exists | Submit existing username | Block form, show error |  |  |
| Auth-04 | Sign up with valid data | Register successfully | No duplicate email/user | Submit valid form | User created, verify email prompt |  |  |
| Auth-05 | Sign in with invalid credentials | Block login with wrong data | User on login page | Submit invalid creds | Show error, no session |  |  |
| Auth-06 | Sign in with unverified email | Block login for unverified accounts | Unverified account | Submit valid creds | Show verify email message |  |  |
| Auth-07 | Verify email | Activate account via email | Email received | Click verification link | Account verified, redirect |  |  |
| Auth-08 | Resend verification email | Allow resending of email | Unverified account | Click resend | Email sent again |  |  |
| Auth-09 | Forgot password with invalid email | Prevent data leak | User on reset page | Submit invalid email | Generic message shown |  |  |
| Auth-10 | Forgot password with valid email | Send reset link | Email registered | Submit valid email | Email with link sent |  |  |
| Auth-11 | Sign in with verified email | Allow valid login | Verified account exists | Submit valid creds | Redirect to dashboard |  |  |
| Auth-12 | Change password (valid old) | Allow password change | User logged in | Submit valid old + new | Success message |  |  |
| Auth-13 | Change password (wrong old) | Block wrong old password | User logged in | Submit wrong old password | Show error message |  |  |
| Auth-14 | Access denied pages while logged in | Restrict access by role | User logged in, wrong role | Visit admin page | Show error or redirect |  |  |

---

## 📊 Summary Table – By Test Case

| Test Case ID | Title | Result | Notes |
|--------------|-------|--------|-------|
| Auth-01 | Access Different Pages Without Being Logged In |        |       |
| Auth-02 | Sign Up with Used Email |        |       |
| Auth-03 | Sign Up with Used Username |        |       |
| Auth-04 | Sign Up with Valid Data |        |       |
| Auth-05 | Sign In with Invalid Credentials |        |       |
| Auth-06 | Sign In with Unverified Email |        |       |
| Auth-07 | Verify Email |        |       |
| Auth-08 | Resend Verification Email |        |       |
| Auth-09 | Forgot Password with Invalid Email |        |       |
| Auth-10 | Forgot Password with Valid Email |        |       |
| Auth-11 | Sign In with Verified Email |        |       |
| Auth-12 | Change Password with Valid Old Password |        |       |
| Auth-13 | Change Password with Invalid Old Password |        |       |
| Auth-14 | Access Denied Pages with Being Logged In |        |       |

---

## 📈 Summary Table – By Result

| Result     | Count |
|------------|-------|
| ✅ PASS     |       |
| ❌ FAIL     |       |
| ⚠️ BLOCKED |       |
| 🔄 RETEST  |       |
| ⏭️ SKIPPED |       |

---

## 🧾 Legend

* ✅ **PASS** – Test executed successfully  
* ❌ **FAIL** – Test failed to meet expected results  
* ⚠️ **BLOCKED** – Cannot execute due to dependencies  
* 🔄 **RETEST** – Needs re-execution after fixes  
* ⏭️ **SKIPPED** – Skipped (not applicable)
