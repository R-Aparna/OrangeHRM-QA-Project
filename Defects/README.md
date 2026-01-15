# Login Feature – Defects

## DEF-01: Username Case Sensitivity Mismatch
**Module:** Login  
**Severity:** Medium  
**Priority:** Medium  

**Description:**  
Login page indicates username must be "Admin", however login is successful when lowercase "admin" is entered.

**Pre-condition:** User is on Login page  

**Steps to Reproduce:**
1. Enter username as "admin"
2. Enter valid password
3. Click Login button

**Expected Result:**  
Username should be case-sensitive and reject lowercase input  
OR UI should clearly indicate username is not case-sensitive

**Actual Result:**  
User is logged in successfully with lowercase username

**Status:** Open

## DEF-02: Space Character Handling Inconsistent Between Username and Password Fields
**Module:** Login  
**Severity:** Low  
**Priority:** Medium  

**Description:**  
Username and password fields handle space characters inconsistently.

**Pre-condition:** User is on Login page  

**Steps to Reproduce:**
1. Press space bar in username field
2. Observe input behavior
3. Press space bar in password field
4. Observe input behavior

**Expected Result:**  
Both fields should handle space characters consistently

**Actual Result:**  
- Username field ignores space input (appears blank)
- Password field accepts space input and displays masked characters

**Status:** Open

## DEF-03: Password Field Accepts Space-Only Input
**Module:** Login  
**Severity:** Low  
**Priority:** Medium  

**Description:**  
Password field allows space-only input, which may lead to invalid authentication attempts.

**Pre-condition:** User is on Login page  

**Steps to Reproduce:**
1. Enter valid username
2. Enter spaces only in password field
3. Click Login button

**Expected Result:**  
System should reject space-only input as invalid

**Actual Result:**  
Password field accepts space input and masks it

**Status:** Open

