# [BUG-001] Soft Keyboard Overlays "Login" Button After Validation Error and Prevents Dismissal

**Component:** Authentication / Login Screen UI  
**Priority:** High  
**Severity:** High Severity  
**Environment:** Apple iPhone 13; iOS version 16.4.1; App Version 2.0.0 (Build 1.1.12)  
**Reproducibility Rate:** 100%  

## Preconditions
1. The application is successfully installed on the mobile device.
2. The user is on the Authorization (Login) page.

## Steps to Reproduce
1. Enter an invalid email address into the "Email" input field.
2. Enter any arbitrary password into the "Password" input field.
3. Tap the "Login" button.
4. Tap back into the "Email" field to correct the invalid input data.
5. Enter a validly formatted email address.

## Expected Result
After correcting the input data, the soft keyboard should automatically dismiss, or the user should be allowed to scroll the screen/tap outside the input area to collapse the keyboard, ensuring the "Login" button remains visible, interactive, and accessible.

## Actual Result
The soft keyboard remains active and locked on the screen, completely overlaying the bottom section of the viewport and blocking the "Login" button. Scrolling the page is impossible, and tapping outside the input fields (Tap outside) fails to trigger a keyboard dismissal or collapse.
