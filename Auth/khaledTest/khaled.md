# ✅ Authentication Test Cases

---

## 📋 Full Test Case Table

| Test Case ID | Title | Objective | Preconditions | Steps | Expected Results | Result | Justification |
|--------------|-------|-----------|----------------|-------|------------------|--------|----------------|
| Auth-01 | Access pages unauthenticated | Block unauthenticated access | User not logged in | Try /dashboard, settings, admin | Redirect to login, no data shown | ✅ PASS | User redirected to login |
| Auth-02 | Sign up with used email | Prevent duplicate email registration | Email exists | Submit existing email | Block form, show error | ✅ PASS | Error: "Email already exists" |
| Auth-03 | Sign up with used username | Prevent duplicate usernames | Username exists | Submit existing username | Block form, show error | ✅ PASS | Error: "Username already exists" |
| Auth-04 | Sign up with valid data | Register successfully | No duplicate email/user | Submit valid form | User created, verify email prompt | ✅ PASS | Redirected to email verification |
| Auth-05 | Sign in with invalid credentials | Block login with wrong data | User on login page | Submit invalid creds | Show error, no session | ✅ PASS | Error: "Login failed..." |
| Auth-06 | Sign in with unverified email | Block login for unverified accounts | Unverified account | Submit valid creds | Show verify email message | ✅ PASS | Error: "Login failed..." |
| Auth-07 | Verify email | Activate account via email | Email received | Click verification link | Account verified, redirect | ✅ PASS | Worked as expected |
| Auth-08 | Resend verification email | Allow resending of email | Unverified account | Click resend | Email sent again | ✅ PASS | User can resend email to same or another address |
| Auth-09 | Forgot password with invalid email | Prevent data leak | User on reset page | Submit invalid email | Generic message shown | ✅ PASS | Specific error: "Email does not have an account" |
| Auth-10 | Forgot password with valid email | Send reset link | Email registered | Submit valid email | Email with link sent | ✅ PASS | Email sent but marked as spam ⚠️ |
| Auth-11 | Sign in with verified email | Allow valid login | Verified account exists | Submit valid creds | Redirect to dashboard | ✅ PASS | Redirected to "/admin/user" |
| Auth-12 | Change password (valid old) | Allow password change | User logged in | Submit valid old + new | Success message | ✅ PASS | Worked as expected |
| Auth-13 | Change password (wrong old) | Block wrong old password | User logged in | Submit wrong old password | Show error message | ✅ PASS | Error shown: "Incorrect password..." |
| Auth-14 | Access denied pages while logged in | Restrict access by role | User logged in, wrong role | Visit admin page | Show error or redirect | ✅ PASS | Redirected to "/AccessDenied" |

---

## 📊 Summary Table – By Test Case

| Test Case ID | Title | Result | Notes |
|--------------|-------|--------|-------|
| Auth-01 | Access Different Pages Without Being Logged In | ✅ PASS | |
| Auth-02 | Sign Up with Used Email | ✅ PASS | |
| Auth-03 | Sign Up with Used Username | ✅ PASS | |
| Auth-04 | Sign Up with Valid Data | ✅ PASS | |
| Auth-05 | Sign In with Invalid Credentials | ✅ PASS | |
| Auth-06 | Sign In with Unverified Email | ✅ PASS | |
| Auth-07 | Verify Email | ✅ PASS | |
| Auth-08 | Resend Verification Email | ✅ PASS | |
| Auth-09 | Forgot Password with Invalid Email | ✅ PASS | |
| Auth-10 | Forgot Password with Valid Email | ✅ PASS | Reset link sent, but email was delivered to spam ⚠️ |
| Auth-11 | Sign In with Verified Email | ✅ PASS | |
| Auth-12 | Change Password with Valid Old Password | ✅ PASS | |
| Auth-13 | Change Password with Invalid Old Password | ✅ PASS | |
| Auth-14 | Access Denied Pages with Being Logged In | ✅ PASS | |

---

## 📈 Summary Table – By Result

| Result     | Count |
|------------|-------|
| ✅ PASS     | 14    |
| ❌ FAIL     | 0     |
| ⚠️ BLOCKED | 0     |
| 🔄 RETEST  | 0     |
| ⏭️ SKIPPED | 0     |

---

## 🧾 Legend

* ✅ **PASS** – Test executed successfully  
* ❌ **FAIL** – Test failed to meet expected results  
* ⚠️ **BLOCKED** – Cannot execute due to dependencies  
* 🔄 **RETEST** – Needs re-execution after fixes  
* ⏭️ **SKIPPED** – Skipped (not applicable)
