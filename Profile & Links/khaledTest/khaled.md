# 👤 Profile and Links Test Cases

---

## 📋 Full Test Case Table

| Test Case ID | Title | Objective | Preconditions | Steps | Expected Results | Result | Justification |
|--------------|-------|-----------|----------------|-------|------------------|--------|----------------|
| Profile-01 | Upgrade Plan to a New One | Ensure users can upgrade to a different plan successfully | Logged-in user with free/lower-tier plan | Go to upgrade section → choose new plan → confirm | Plan is updated with confirmation | ✅ PASS | |
| Profile-02 | Upgrade Plan with the Same Plan | Prevent selecting same plan | User has active plan | Try upgrading to current plan | Block action with message | ✅ PASS | Cannot pick existing plan |
| Profile-03 | Pick a Cover Picture | Allow cover upload | User logged in | Go to profile → upload cover image | Image is shown and saved | ✅ PASS | |
| Profile-04 | Change Cover Picture | Replace existing cover | Existing cover image | Upload new cover | Cover updates immediately | ✅ PASS | |
| Profile-05 | Upload Invalid Cover Image | Prevent invalid cover formats | Logged-in user | Try uploading non-image file | Upload rejected with error | ✅ PASS | Proper validation error shown |
| Profile-06 | Pick a Profile Picture | Set a profile image | User logged in | Upload avatar image | Avatar displayed and saved | ✅ PASS | |
| Profile-07 | Change Profile Picture | Update existing avatar | Has profile picture | Upload new image → save | Avatar updates correctly | ✅ PASS | |
| Profile-08 | Upload Invalid Profile Picture | Prevent invalid image formats | User logged in | Upload PDF file as image | Validation and error shown | ❌ FAIL | Error message not user-friendly |
| Profile-09 | Update Profile with Valid Info | Update personal info | User logged in | Change name/bio → save | Confirmation shown | ✅ PASS | |
| Profile-10 | Update Profile with Invalid Info | Block invalid input | User logged in | Enter malicious data → submit | Error messages shown | ✅ PASS | Strong validation enforced |
| Profile-11 | Disable Public Profile & Test Search | Hide profile from search | Profile has search toggle | Disable visibility → search from another account | Profile not visible | ✅ PASS | |
| Profile-12 | Upload CV | Upload resume in profile | User logged in | Upload valid PDF | Confirmation shown | ✅ PASS | |
| Profile-13 | Replace Existing CV | Replace old resume | Existing CV uploaded | Upload new CV → save | Old CV replaced | ❌ FAIL | Error: "Error updating CV" |
| Profile-14 | Add Custom Link | Add link to profile | Logged-in user | Add URL + label | Link added and visible | ✅ PASS | |
| Profile-15 | Update Custom Link | Edit existing link | Link exists | Change URL/label → save | Link updated correctly | ✅ PASS | |
| Profile-16 | Add Social Media Account | Add social platform link | Logged-in user | Add Instagram, LinkedIn | Social icon shown | ✅ PASS | x.com not accepted for X |
| Profile-17 | Update Social Media Account | Edit social URLs | Links already exist | Edit → save | Updates saved | ✅ PASS | |
| Profile-18 | Delete Phone Number | Remove phone info | Phone number saved | Remove and save | Number deleted | ✅ PASS | |
| Profile-19 | Add a New Phone Number | Add phone number | No phone exists | Add valid number → save | Saved correctly | ✅ PASS | |
| Profile-20 | Add Email | Add contact email to profile | User logged in | Add email → save | Email saved | ✅ PASS | |
| Profile-21 | Modify Email | Edit email info | Email already saved | Edit → save | Email updated | ✅ PASS | |
| Profile-22 | Delete Email | Remove saved email | At least one email exists | Delete → save | Email removed | ✅ PASS | |
| Profile-23 | Show CV in Profile | Enable preview of CV | CV already uploaded | Click "View CV" | PDF preview shown | ✅ PASS | |
| Profile-24 | Download CV | Download CV from profile | CV uploaded | Click "Download CV" | File downloaded | ✅ PASS | |
| Profile-25 | QR Code Test | Test QR functionality | QR generated | Scan with phone | Profile opens in browser | ✅ PASS | |
| Profile-26 | vCard Test | Save contact from vCard | User has complete info | Click "Save Contact" | vCard opens with info | ✅ PASS | |

---

## 📊 Summary Table – By Test Case

| Test Case ID | Title                                   | Result | Notes |
|--------------|-----------------------------------------|--------|-------|
| Profile-01   | Upgrade Plan to a New One               | ✅ PASS | |
| Profile-02   | Upgrade Plan with the Same Plan         | ✅ PASS | Cannot pick current plan |
| Profile-03   | Pick a Cover Picture                    | ✅ PASS | User can't crop the image |
| Profile-04   | Change Cover Picture                    | ✅ PASS | |
| Profile-05   | Upload Invalid Cover Image              | ✅ PASS | Validation works correctly |
| Profile-06   | Pick a Profile Picture                  | ✅ PASS | User can't crop the image |
| Profile-07   | Change Profile Picture                  | ✅ PASS | |
| Profile-08   | Upload Invalid Profile Picture          | ❌ FAIL | Poor UX on error message |
| Profile-09   | Update Profile with Valid Info          | ✅ PASS | |
| Profile-10   | Update Profile with Invalid Info        | ✅ PASS | Strong input validation |
| Profile-11   | Disable Public Profile & Test Search    | ✅ PASS | |
| Profile-12   | Upload CV                               | ✅ PASS | |
| Profile-13   | Replace Existing CV                     | ❌ FAIL | Error shown when uploading |
| Profile-14   | Add Custom Link                         | ✅ PASS | |
| Profile-15   | Update Custom Link                      | ✅ PASS | |
| Profile-16   | Add Social Media Account                | ✅ PASS | x.com not accepted |
| Profile-17   | Update Social Media Account             | ✅ PASS | |
| Profile-18   | Delete Phone Number                     | ✅ PASS | |
| Profile-19   | Add a New Phone Number                  | ✅ PASS | |
| Profile-20   | Add Email                               | ✅ PASS | |
| Profile-21   | Modify Email                            | ✅ PASS | |
| Profile-22   | Delete Email                            | ✅ PASS | |
| Profile-23   | Show CV in Profile                      | ✅ PASS | |
| Profile-24   | Download CV                             | ✅ PASS | |
| Profile-25   | QR Code Test                            | ✅ PASS | |
| Profile-26   | vCard Test                              | ✅ PASS | |

---

## 📈 Summary Table – By Result

| Result     | Count |
|------------|-------|
| ✅ PASS     | 24    |
| ❌ FAIL     | 2     |
| ⚠️ BLOCKED | 0     |
| 🔄 RETEST  | 0     |
| ⏭️ SKIP    | 0     |

---

## 🗂️ Legend

- ✅ **PASS** – Test executed successfully  
- ❌ **FAIL** – Test failed to meet expected results  
- ⚠️ **BLOCKED** – Cannot execute due to dependencies  
- 🔄 **RETEST** – Needs re-execution after fixes  
- ⏭️ **SKIP** – Skipped (not applicable)
