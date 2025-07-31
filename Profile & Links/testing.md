# 👤 Profile and Links Test Cases

---

## 📋 Full Test Case Table

| Test Case ID | Title | Objective | Preconditions | Steps | Expected Results | Result | Justification |
|--------------|-------|-----------|----------------|-------|------------------|--------|----------------|
| Profile-01 | Upgrade Plan to a New One | Ensure users can upgrade to a different plan successfully | Logged-in user with free/lower-tier plan | Go to upgrade section → choose new plan → confirm | Plan is updated with confirmation |  |  |
| Profile-02 | Upgrade Plan with the Same Plan | Prevent selecting same plan | User has active plan | Try upgrading to current plan | Block action with message |  |  |
| Profile-03 | Pick a Cover Picture | Allow cover upload | User logged in | Go to profile → upload cover image | Image is shown and saved |  |  |
| Profile-04 | Change Cover Picture | Replace existing cover | Existing cover image | Upload new cover | Cover updates immediately |  |  |
| Profile-05 | Upload Invalid Cover Image | Prevent invalid cover formats | Logged-in user | Try uploading non-image file | Upload rejected with error |  |  |
| Profile-06 | Pick a Profile Picture | Set a profile image | User logged in | Upload avatar image | Avatar displayed and saved |  |  |
| Profile-07 | Change Profile Picture | Update existing avatar | Has profile picture | Upload new image → save | Avatar updates correctly |  |  |
| Profile-08 | Upload Invalid Profile Picture | Prevent invalid image formats | User logged in | Upload PDF file as image | Validation and error shown |  |  |
| Profile-09 | Update Profile with Valid Info | Update personal info | User logged in | Change name/bio → save | Confirmation shown |  |  |
| Profile-10 | Update Profile with Invalid Info | Block invalid input | User logged in | Enter malicious data → submit | Error messages shown |  |  |
| Profile-11 | Disable Public Profile & Test Search | Hide profile from search | Profile has search toggle | Disable visibility → search from another account | Profile not visible |  |  |
| Profile-12 | Upload CV | Upload resume in profile | User logged in | Upload valid PDF | Confirmation shown |  |  |
| Profile-13 | Replace Existing CV | Replace old resume | Existing CV uploaded | Upload new CV → save | Old CV replaced |  |  |
| Profile-14 | Add Custom Link | Add link to profile | Logged-in user | Add URL + label | Link added and visible |  |  |
| Profile-15 | Update Custom Link | Edit existing link | Link exists | Change URL/label → save | Link updated correctly |  |  |
| Profile-16 | Add Social Media Account | Add social platform link | Logged-in user | Add Instagram, LinkedIn | Social icon shown |  |  |
| Profile-17 | Update Social Media Account | Edit social URLs | Links already exist | Edit → save | Updates saved |  |  |
| Profile-18 | Delete Phone Number | Remove phone info | Phone number saved | Remove and save | Number deleted |  |  |
| Profile-19 | Add a New Phone Number | Add phone number | No phone exists | Add valid number → save | Saved correctly |  |  |
| Profile-20 | Add Email | Add contact email to profile | User logged in | Add email → save | Email saved |  |  |
| Profile-21 | Modify Email | Edit email info | Email already saved | Edit → save | Email updated |  |  |
| Profile-22 | Delete Email | Remove saved email | At least one email exists | Delete → save | Email removed |  |  |
| Profile-23 | Show CV in Profile | Enable preview of CV | CV already uploaded | Click "View CV" | PDF preview shown |  |  |
| Profile-24 | Download CV | Download CV from profile | CV uploaded | Click "Download CV" | File downloaded |  |  |
| Profile-25 | QR Code Test | Test QR functionality | QR generated | Scan with phone | Profile opens in browser |  |  |
| Profile-26 | vCard Test | Save contact from vCard | User has complete info | Click "Save Contact" | vCard opens with info |  |  |

---

## 📊 Summary Table – By Test Case

| Test Case ID | Title                                   | Result | Notes |
|--------------|-----------------------------------------|--------|-------|
| Profile-01   | Upgrade Plan to a New One               |        |       |
| Profile-02   | Upgrade Plan with the Same Plan         |        |       |
| Profile-03   | Pick a Cover Picture                    |        |       |
| Profile-04   | Change Cover Picture                    |        |       |
| Profile-05   | Upload Invalid Cover Image              |        |       |
| Profile-06   | Pick a Profile Picture                  |        |       |
| Profile-07   | Change Profile Picture                  |        |       |
| Profile-08   | Upload Invalid Profile Picture          |        |       |
| Profile-09   | Update Profile with Valid Info          |        |       |
| Profile-10   | Update Profile with Invalid Info        |        |       |
| Profile-11   | Disable Public Profile & Test Search    |        |       |
| Profile-12   | Upload CV                               |        |       |
| Profile-13   | Replace Existing CV                     |        |       |
| Profile-14   | Add Custom Link                         |        |       |
| Profile-15   | Update Custom Link                      |        |       |
| Profile-16   | Add Social Media Account                |        |       |
| Profile-17   | Update Social Media Account             |        |       |
| Profile-18   | Delete Phone Number                     |        |       |
| Profile-19   | Add a New Phone Number                  |        |       |
| Profile-20   | Add Email                               |        |       |
| Profile-21   | Modify Email                            |        |       |
| Profile-22   | Delete Email                            |        |       |
| Profile-23   | Show CV in Profile                      |        |       |
| Profile-24   | Download CV                             |        |       |
| Profile-25   | QR Code Test                            |        |       |
| Profile-26   | vCard Test                              |        |       |

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

## 🗂️ Legend

- ✅ **PASS** – Test executed successfully  
- ❌ **FAIL** – Test failed to meet expected results  
- ⚠️ **BLOCKED** – Cannot execute due to dependencies  
- 🔄 **RETEST** – Needs re-execution after fixes  
- ⏭️ **SKIP** – Skipped (not applicable)
