Login Feature Test Plan

## 1. Project Overview
This Test Plan covers the **Login functionality** of the OrangeHRM demo web application.  
The purpose is to validate **functional correctness, usability, security, and error handling** for different types of user inputs.

## 2. Scope of Testing
**In Scope:**
- Login with valid credentials
- Login with invalid credentials
- Password masking and visibility
- Required field validations
- Case sensitivity of username
- Space character handling in username and password
- Error message validation
- Post-error login behavior

**Out of Scope:**
- Forgot Password functionality
- Multi-user sessions
- Admin or role-based access beyond login
- Integration with other modules

## 3. Pre-requisites
- User is on the OrangeHRM Login page
- Browser: Chrome / Firefox / Edge (latest versions)
- Internet connection stable
- Valid credentials available for testing (`Username: Admin`, `Password: admin123`)

## 4. Test Approach
- **Manual Testing** will be performed for all scenarios  
- **Positive Testing:** Valid username/password combination  
- **Negative Testing:** Invalid username/password, empty fields, extra spaces  
- **UI Testing:** Password masking, required field messages  
- **Edge Cases:** Case sensitivity, trailing spaces  

## 5. Test Scenarios
1. Login with valid credentials  
2. Login with valid username / invalid password  
3. Login with invalid username / valid password  
4. Login with invalid username / invalid password  
5. Password masking validation  
6. Required field validation when username/password is empty  
7. Behavior when trailing/leading spaces are entered in username/password  
8. Post-error login correction and login success  

## 6. Test Data
| Scenario | Username | Password |
|----------|----------|----------|
| Valid Login | Admin | admin123 |
| Invalid Password | Admin | admin |
| Invalid Username | admin1 | admin123 |
| Invalid Username & Password | admin1 | admin1 |
| Empty Fields | (blank) | (blank) |

## 7. Entry & Exit Criteria
**Entry Criteria:**
- OrangeHRM login page accessible  
- Test data ready  

**Exit Criteria:**
- All test scenarios executed  
- All defects logged and reviewed  
- Critical defects resolved  

## 8. Deliverables
- Test Plan document (this file)  
- Test Cases (Test-Cases folder)  
- Defects log (Defects folder)  

## 9. Assumptions & Risks
**Assumptions:**
- Application is in a stable environment  
- Testers have access to credentials  

**Risks:**
- UI changes may require test updates  
- Internet/browser issues may affect testing  

