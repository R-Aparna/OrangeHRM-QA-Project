# Login Feature – Test Cases

## TC-01: Login with Valid Credentials
**Pre-condition:** User is on Login page  
**Test Data:** Username = Admin, Password = admin123  

**Steps:**
1. Enter valid username
2. Enter valid password
3. Click Login button

**Expected Result:**
- User is successfully logged in
- User is redirected to Dashboard page

## TC-02: Login with Valid Username and Invalid Password
**Pre-condition:** User is on Login page  
**Test Data:** Username = Admin, Password = admin  

**Steps:**
1. Enter valid username
2. Enter invalid password
3. Click Login button

**Expected Result:**
- Error message displayed: *"Invalid Credentials"*
- User remains on Login page

## TC-03: Login with Invalid Username and Valid Password
**Pre-condition:** User is on Login page  
**Test Data:** Username = admin1, Password = admin123  

**Steps:**
1. Enter invalid username
2. Enter valid password
3. Click Login button

**Expected Result:**
- Error message displayed: *"Invalid Credentials"*
- User remains on Login page

## TC-04: Login with Invalid Username and Invalid Password
**Pre-condition:** User is on Login page  
**Test Data:** Username = admin1, Password = admin1  

**Steps:**
1. Enter invalid username
2. Enter invalid password
3. Click Login button

**Expected Result:**
- Error message displayed: *"Invalid Credentials"*
- User remains on Login page

## TC-05: Password Masking Validation
**Pre-condition:** User is on Login page  

**Steps:**
1. Enter username
2. Enter password

**Expected Result:**
- Password characters are masked (hidden)

## TC-06: Required Field Validation
**Pre-condition:** User is on Login page  

**Steps:**
1. Leave username blank
2. Leave password blank
3. Click Login button

**Expected Result:**
- "Required" field message displayed below both fields in red

## TC-07: Required Message Disappears on Input
**Pre-condition:** "Required" field error is displayed  

**Steps:**
1. Enter value in username field

**Expected Result:**
- "Required" field message disappears immediately

## TC-08: Username Case Sensitivity Validation
**Pre-condition:** User is on Login page  
**Test Data:** Username = admin, Password = admin123  

**Steps:**
1. Enter username in lowercase
2. Enter valid password
3. Click Login button

**Expected Result:**
- User is logged in successfully
- Username is **not case-sensitive**

## TC-09: Space Handling in Username Field
**Pre-condition:** User is on Login page  

**Steps:**
1. Press space bar in username field

**Expected Result:**
- Cursor moves but field appears blank
- Space-only input is ignored

## TC-10: Space Handling in Password Field
**Pre-condition:** User is on Login page  

**Steps:**
1. Press space bar in password field

**Expected Result:**
- Masked characters appear
- Space is accepted as input

## TC-11: Correcting Invalid Credentials and Login
**Pre-condition:** Invalid credentials error is displayed  

**Steps:**
1. Enter correct username and password
2. Click Login button

**Expected Result:**
- User logs in successfully
- Error message is cleared
