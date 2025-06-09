### BUG-001: Username field is not case-sensitive

**Bug ID:** BUG-001  
**Title:** Username field is not case-sensitive  
**Test Scenario**: Verify Login Functionality  
**Environment**:  
- Device: Desktop
- OS: Windows 11 Home  
- Browser: Google Chrome 125.0.6422.113 (64-bit)  
- Application URL: https://opensource-demo.orangehrmlive.com
  
**Severity**: Medium  
**Priority**: High  

---

### Description:
Login system accepts both `Admin` and `admin` as valid usernames with the same password (`admin123`). The system appears to treat the username field as **case-insensitive**, which may lead to ambiguity or potential security concerns.

---

### Steps to Reproduce:
1. Go to [Login Page](https://opensource-demo.orangehrmlive.com)
2. Enter:
   - Username: `admin`
   - Password: `admin123`
3. Click `Login`

---

### Expected Result:
Only `Admin` (as displayed) should be accepted as valid if usernames are case-sensitive.

---

### Actual Result:
Both `Admin` and `admin` allow successful login.

---

### Visual Proof:
https://github.com/user-attachments/assets/44893af9-8486-4130-a7b4-2f7a76a661dd
