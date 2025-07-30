# Authentication Test Cases

---

### Auth-01: Access Different Pages Without Being Logged In

**Test Objective:**
Ensure that restricted pages cannot be accessed by unauthenticated users.

**Preconditions:**

* User is not logged in
* Application routes are secured properly

**Test Steps:**

1. Try accessing a protected route (e.g., /dashboard)
2. Try accessing user settings page
3. Try accessing admin-only pages

**Expected Results:**

* The user is redirected to the login page
* No restricted data is shown

**Test Result:**
✅ **PASS**

**Justification:** worked as expected the user got redirected to the login page 
---

### Auth-02: Sign Up with Used Email

**Test Objective:**
Ensure system prevents sign-up with an email already in use

**Preconditions:**

* The email is already registered in the database

**Test Steps:**

1. Navigate to the sign-up page
2. Enter an already-registered email
3. Fill out other fields with valid data
4. Submit the form

**Expected Results:**

* Form submission is blocked
* A clear error message is shown (e.g., "Email already exists")

**Test Result:**
✅ **PASS**

**Justification:** worked as expected an error message is shown "A user with this email already exists."

---

### Auth-03: Sign Up with Used Username

**Test Objective:**
Ensure system prevents sign-up with a taken username

**Preconditions:**

* Username is already used by another account

**Test Steps:**

1. Navigate to the sign-up page
2. Enter a username already in use
3. Fill out other fields with valid data
4. Submit the form

**Expected Results:**

* Form submission is blocked
* A clear error message is displayed (e.g., "Username already taken")

**Test Result:**
✅ **PASS**

**Justification:** worked as expected an error message is shown "A user with this username already exists."

---

### Auth-04: Sign Up with Valid Data

**Test Objective:**
Verify that users can register successfully with valid credentials

**Preconditions:**

* No duplicate email/username

**Test Steps:**

1. Navigate to the sign-up page
2. Fill in all required fields with valid information
3. Submit the form

**Expected Results:**

* The user account is created
* User is prompted to verify their email

**Test Result:**
⚠️ **BLOCKED**

**Justification:**

---

### Auth-05: Sign In with Invalid Credentials

**Test Objective:**
Ensure that users cannot log in with incorrect email or password

**Preconditions:**

* User is on the login page

**Test Steps:**

1. Enter an invalid email or password
2. Click on "Sign In"

**Expected Results:**

* Authentication fails
* Error message is shown (e.g., "Invalid credentials")
* No session or token is saved

**Test Result:**
✅ **PASS**

**Justification:**worked as expected an error message is shown "Login failed. Please check your credentials."

---

### Auth-06: Sign In with Unverified Email

**Test Objective:**
Ensure unverified users are blocked from accessing the platform

**Preconditions:**

* A user account exists but hasn't verified the email

**Test Steps:**

1. Enter valid credentials of unverified account
2. Click "Sign In"

**Expected Results:**

* Login is denied
* A message prompts user to verify their email

**Test Result:**
⚠️ **BLOCKED**

**Justification:**

---

### Auth-07: Verify Email

**Test Objective:**
Verify the user can activate their account through the email link

**Preconditions:**

* User has received a verification email

**Test Steps:**

1. Open the email
2. Click the verification link

**Expected Results:**

* Account becomes verified
* Redirects to login or home page with success message

**Test Result:**
⚠️ **BLOCKED**

**Justification:**

---

### Auth-08: Resend Verification Email

**Test Objective:**
Ensure the user can resend verification if the first one was not received

**Preconditions:**

* User has signed up but hasn't verified their email

**Test Steps:**

1. Navigate to login or verify page
2. Click "Resend Verification Email"

**Expected Results:**

* Verification email is sent again
* Confirmation message is shown

**Test Result:**
⚠️ **BLOCKED**

**Justification:**

---

### Auth-09: Forgot Password with Invalid Email

**Test Objective:**
Ensure system handles invalid/non-existent email in password reset

**Preconditions:**

* User is on the "Forgot Password" page

**Test Steps:**

1. Enter a random or invalid email
2. Click "Send Reset Link"

**Expected Results:**

* A message is shown like "If an account exists, a reset link will be sent"
* No data is leaked about registered accounts

**Test Result:** 
✅ **PASS**

**Justification:** worked better than expected an error message is shown "This email does not have an account."

---

### Auth-10: Forgot Password with Valid Email

**Test Objective:**
Verify reset link is sent for valid registered email

**Preconditions:**

* User email is already registered

**Test Steps:**

1. Navigate to "Forgot Password"
2. Enter valid registered email
3. Click "Send Reset Link"

**Expected Results:**

* Email with reset link is received
* Message confirms that instructions were sent

**Test Result:**
✅ **PASS**

**Justification:** worked as expected with minor problem an reset link was sent from "contact@idigics.com" but "the email was put in spam⚠️"

---

### Auth-11: Sign In with Verified Email

**Test Objective:**
Allow login when credentials are correct and email is verified

**Preconditions:**

* A verified account exists

**Test Steps:**

1. Navigate to login
2. Enter valid credentials
3. Click "Sign In"

**Expected Results:**

* User is redirected to dashboard or home
* Token/session is saved

**Test Result:**
✅ **PASS**

**Justification:** worked as expected the user is redirected to "/admin/user"

---

### Auth-12: Change Password with Valid Old Password

**Test Objective:**
Ensure password change works with correct old password

**Preconditions:**

* User is logged in

**Test Steps:**

1. Go to account settings
2. Enter current password and new password
3. Submit

**Expected Results:**

* Password is updated
* Success message is shown

**Test Result:**
✅ **PASS**

**Justification:**

---

### Auth-13: Change Password with Invalid Old Password

**Test Objective:**
Ensure password change fails with incorrect old password

**Preconditions:**

* User is logged in

**Test Steps:**

1. Go to change password section
2. Enter wrong old password and new password
3. Submit

**Expected Results:**

* Password is not changed
* Error message is shown (e.g., "Old password incorrect")

**Test Result:**
✅ **PASS**

**Justification:** worked as expected an error message was shown "Incorrect password please try again later."



---

### Auth-14: Access Denied Pages with Being Logged In

**Test Objective:**
Ensure users cannot access unauthorized routes despite being logged in

**Preconditions:**

* User is logged in but not an admin (or appropriate role)

**Test Steps:**

1. Try visiting admin-only page
2. Try accessing another role-restricted area

**Expected Results:**

* Access is denied
* A proper error or redirect is provided

**Test Result:**
✅ **PASS**

**Justification:** worked as expected the user got redirected to "/AccessDenied" 

---

## 🔍 Test Execution Summary

| Test Case ID | Title | Result | Notes |
|--------------|-------|--------|-------|
| Auth-01 | Access Different Pages Without Being Logged In | ✅ PASS |  |
| Auth-02 | Sign Up with Used Email | ✅ PASS |  |
| Auth-03 | Sign Up with Used Username | ✅ PASS |  |
| Auth-04 | Sign Up with Valid Data | ⚠️ BLOCKED | Missing result and justification |
| Auth-05 | Sign In with Invalid Credentials | ✅ PASS | |
| Auth-06 | Sign In with Unverified Email | ⚠️ BLOCKED | Missing result and justification |
| Auth-07 | Verify Email | ⚠️ BLOCKED | Missing result and justification |
| Auth-08 | Resend Verification Email | ⚠️ BLOCKED | Missing result and justification |
| Auth-09 | Forgot Password with Invalid Email | ✅ PASS | |
| Auth-10 | Forgot Password with Valid Email | ✅ PASS |Reset link sent, but email went to spam ⚠️ |
| Auth-11 | Sign In with Verified Email | ✅ PASS | |
| Auth-12 | Change Password with Valid Old Password | ✅ PASS |  |
| Auth-13 | Change Password with Invalid Old Password | ✅ PASS |  |
| Auth-14 | Access Denied Pages with Being Logged In | ✅ PASS |  |

---

### Legend

* ✅ **PASS** – Test executed successfully
* ❌ **FAIL** – Test failed to meet expected results
* ⚠️ **BLOCKED** – Cannot execute due to dependencies
* 🔄 **RETEST** – Needs re-execution after fixes
* ⏭️ **SKIP** – Skipped (not applicable)
