# 👤 Profile and Links Test Cases

---

### Profile-01: Upgrade Plan to a New One

**Test Objective:**  
Ensure users can upgrade to a different plan successfully.

**Preconditions:**  
- User is logged in  
- Has an active lower-tier or free plan

**Test Steps:**  
1. Go to upgrade plan section  
2. Choose a higher-tier plan  
3. Confirm upgrade

**Expected Results:**  
- Plan is updated  
- Confirmation and billing info are shown

**Test Result:**  
✅ **PASS**  

**Justification:**  

---

### Profile-02: Upgrade Plan with the Same Plan

**Test Objective:**  
Prevent users from upgrading to the same plan they already have.

**Preconditions:**  
- User has an active plan

**Test Steps:**  
1. Go to upgrade page  
2. Select current plan  
3. Click "Upgrade"

**Expected Results:**  
- Upgrade is blocked  
- Message like "You are already on this plan" is shown

**Test Result:**  
✅ **PASS**  

**Justification:** worked better than expected, the user can't pick the plan that he already have.  

---

### Profile-03: Pick a Cover Picture

**Test Objective:**  
Allow users to set a new cover photo

**Test Steps:**  
1. Navigate to profile settings  
2. Upload a valid image as cover

**Expected Results:**  
- Cover photo is displayed  
- Saved successfully

**Test Result:**  
✅ **PASS**  

**Justification:**  

---

### Profile-04: Change Cover Picture

**Test Objective:**  
Ensure users can replace their existing cover image

**Test Steps:**  
1. Upload a different valid image  
2. Save changes

**Expected Results:**  
- Cover is updated and visible instantly

**Test Result:**  
✅ **PASS**  

**Justification:**  

---

### Profile-05: Upload Invalid File as Cover Image

**Test Objective:**  
Block unsupported file formats (e.g., PDF, ZIP)

**Test Steps:**  
1. Try uploading a non-image file

**Expected Results:**  
- Upload is rejected  
- Proper error message is shown

**Test Result:**  
✅ **PASS**

**Justification:** worked as expected an error message is shown "Please select a valid image file"

---

### Profile-06: Pick a Profile Picture

**Test Objective:**  
Allow users to set an avatar/profile photo

**Test Steps:**  
1. Go to profile settings  
2. Upload valid profile image

**Expected Results:**  
- Avatar is displayed  
- Saved successfully

**Test Result:**  
✅ **PASS**  

**Justification:**  

---

### Profile-07: Change Profile Picture

**Test Objective:**  
Ensure users can update their profile image

**Test Steps:**  
1. Upload a different valid image  
2. Save changes

**Expected Results:**  
- Profile image is updated successfully

**Test Result:**  
✅ **PASS**  

**Justification:**  

---

### Profile-08: Upload Invalid File as Profile Picture

**Test Objective:**  
Prevent non-image file uploads

**Test Steps:**  
1. Try uploading invalid format (e.g., PDF)

**Expected Results:**  
- Upload fails with validation error

**Test Result:**  
❌ **FAIL**  

**Justification:** the error message appeard while uploading and when the user tried to  save the new profile image (pdf file) this error is shown "Error saving profile: Server error: 400" it's not good for user experience
...

---

### Profile-09: Update Profile with Valid Info

**Test Objective:**  
Ensure profile fields update correctly

**Test Steps:**  
1. Edit name, bio, location, etc.  
2. Save changes

**Expected Results:**  
- Data is saved  
- Confirmation message shown

**Test Result:**  
✅ **PASS**  

**Justification:**  

---

### Profile-10: Update Profile with Invalid Info

**Test Objective:**  
Prevent invalid data input

**Test Steps:**  
1. Input invalid or malicious data  
2. Submit form

**Expected Results:**  
- Submission blocked  
- Error messages shown

**Test Result:**  
✅ **PASS**

**Justification:** worked better than expected the input fields are controlled and you can't type invalid data 

---

### Profile-11: Disable Public Profile & Test Search

**Test Objective:**  
Ensure disabling search visibility works

**Test Steps:**  
1. Toggle off "Allow profile to be found in search"  
2. Search profile from another account

**Expected Results:**  
- Profile does not appear in search results

**Test Result:**  
✅ **PASS**  

**Justification:**  

---

### Profile-12: Upload CV

**Test Objective:**  
Ensure CV file upload works

**Test Steps:**  
1. Upload a valid PDF as CV

**Expected Results:**  
- CV is uploaded  
- Confirmation message shown

**Test Result:**  
✅ **PASS**  

**Justification:**  

---

### Profile-13: Replace Existing CV

**Test Objective:**  
Allow CV replacement

**Test Steps:**  
1. Upload a new CV  
2. Save changes

**Expected Results:**  
- Old CV is replaced

**Test Result:**  
❌ **FAIL**  

**Justification:** an error message is shown "Error updating CV"

---

### Profile-14: Add Custom Link

**Test Objective:**  
Allow users to add custom links

**Test Steps:**  
1. Go to profile links  
2. Add a new URL and label

**Expected Results:**  
- Link appears in profile  
- Opens correctly

**Test Result:**  
✅ **PASS**  

**Justification:**  

---

### Profile-15: Update Custom Link

**Test Objective:**  
Enable editing of custom link

**Test Steps:**  
1. Edit existing link’s URL or label

**Expected Results:**  
- Changes saved

**Test Result:**  
✅ **PASS**  

**Justification:**  

---

### Profile-16: Add Social Media Account

**Test Objective:**  
Allow linking of social accounts

**Test Steps:**  
1. Add Instagram, LinkedIn, etc.

**Expected Results:**  
- Link shows with icon

**Test Result:**  
✅ **PASS**  

**Justification:** Functionality works as expected, but adding an X (Twitter) account does not accept x.com it only accepts twitter.com

---

### Profile-17: Update Social Media Account

**Test Objective:**  
Allow editing of social URLs

**Test Steps:**  
1. Edit social link  
2. Save changes

**Expected Results:**  
- New links saved

**Test Result:**  
✅ **PASS**  

**Justification:**  

---

### Profile-18: Delete Phone Number

**Test Objective:**  
Allow users to remove phone number

**Test Steps:**  
1. Remove phone  
2. Save

**Expected Results:**  
- Number deleted  
- Confirmation shown

**Test Result:**  
✅ **PASS**    

**Justification:**  

---

### Profile-19: Add a New Phone Number

**Test Objective:**  
Support adding phone contact

**Test Steps:**  
1. Enter valid phone number  
2. Submit

**Expected Results:**  
- Number is saved

**Test Result:**  
✅ **PASS**    

**Justification:**  

---

### Profile-20: Add Email

**Test Objective:**  
add an email to be shown in your profile page so people can contact you with it

**Test Steps:**  
1. Add a new email  
2. Submit

**Expected Results:**  
- Email is saved

**Test Result:**  
✅ **PASS**    

**Justification:**  

---

### Profile-21: Modify Email

**Test Objective:**  
Allow email editing

**Test Steps:**  
1. Edit existing email

**Expected Results:**  
- Email updated

**Test Result:**  
✅ **PASS**    

**Justification:**  

---

### Profile-22: Delete Email

**Test Objective:**  
Allow email deletion

**Test Steps:**  
1. Delete saved email

**Expected Results:**  
- Email removed

**Test Result:**  
✅ **PASS**    

**Justification:**  
...

---

### Profile-23: Show CV in Profile

**Test Objective:**  
Enable CV preview from profile

**Test Steps:**  
1. Click to view CV

**Expected Results:**  
- CV opens in viewer

**Test Result:**  
✅ **PASS**  

**Justification:**  

---

### Profile-24: Download CV

**Test Objective:**  
Allow CV download

**Test Steps:**  
1. Click download button

**Expected Results:**  
- PDF is downloaded

**Test Result:**  
✅ **PASS**    

**Justification:**  

---

### Profile-25: QR Code Test

**Test Objective:**  
Ensure QR code opens correct profile

**Test Steps:**  
1. Scan QR with phone  
2. Confirm redirection

**Expected Results:**  
- Profile opens via scan

**Test Result:**  
✅ **PASS**    

**Justification:**  

---

### Profile-26: vCard Test

**Test Objective:**  
Ensure the vCard saves the correct data as a contact on the phone.

**Test Steps:**  
1. Open the profile on a phone  
2. Press "Save Contact"

**Expected Results:**  
- A new contact should be ready to save in the phone’s contact list, with the corresponding data.

**Test Result:**  
✅ **PASS**    

**Justification:**  

---


## 🔍 Test Execution Summary

| Test Case ID | Title                                   | Result | Notes |
|--------------|-----------------------------------------|--------|-------|
| Profile-01   | Upgrade Plan to a New One               | ✅ PASS |       |
| Profile-02   | Upgrade Plan with the Same Plan         | ✅ PASS | User can't pick current plan |
| Profile-03   | Pick a Cover Picture                    | ✅ PASS | User can't choose what part of the image to be shown |
| Profile-04   | Change Cover Picture                    | ✅ PASS |       |
| Profile-05   | Upload Invalid Cover Image              | ✅ PASS | Validation error shown correctly |
| Profile-06   | Pick a Profile Picture                  | ✅ PASS | User can't choose what part of the image to be shown |
| Profile-07   | Change Profile Picture                  | ✅ PASS |       |
| Profile-08   | Upload Invalid Profile Picture          | ❌ FAIL | Error message not user-friendly |
| Profile-09   | Update Profile with Valid Info          | ✅ PASS |       |
| Profile-10   | Update Profile with Invalid Info        | ✅ PASS | Strong input validation |
| Profile-11   | Disable Public Profile & Test Search    | ✅ PASS |       |
| Profile-12   | Upload CV                               | ✅ PASS |       |
| Profile-13   | Replace Existing CV                     | ❌ FAIL | Error message shown when uploading |
| Profile-14   | Add Custom Link                         | ✅ PASS |       |
| Profile-15   | Update Custom Link                      | ✅ PASS |       |
| Profile-16   | Add Social Media Account                | ✅ PASS | `x.com` not accepted for X (Twitter) |
| Profile-17   | Update Social Media Account             | ✅ PASS |       |
| Profile-18   | Delete Phone Number                     | ✅ PASS |       |
| Profile-19   | Add a New Phone Number                  | ✅ PASS |       |
| Profile-20   | Add Email                               | ✅ PASS |       |
| Profile-21   | Modify Email                            | ✅ PASS |       |
| Profile-22   | Delete Email                            | ✅ PASS |       |
| Profile-23   | Show CV in Profile                      | ✅ PASS |       |
| Profile-24   | Download CV                             | ✅ PASS |       |
| Profile-25   | QR Code Test                            | ✅ PASS |       |

---

### 🗂️ Legend

- ✅ **PASS** – Test executed successfully  
- ❌ **FAIL** – Test failed to meet expected results  
- ⚠️ **BLOCKED** – Cannot execute due to dependencies  
- 🔄 **RETEST** – Needs re-execution after fixes  
- ⏭️ **SKIP** – Skipped (not applicable)  
