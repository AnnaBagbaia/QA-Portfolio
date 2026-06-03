# [BUG-002] "Back" Button Becomes Unresponsive Upon Re-entering the Profile Section

**Component:** Navigation / User Profile Flow  
**Priority:** Medium  
**Severity:** High Severity  
**Environment:** Apple iPhone 13; iOS version 16.4.1; App Version 2.0.0 (Build 1.1.12)  
**Reproducibility Rate:** 100%  

## Preconditions
1. The user is successfully authenticated (Logged in).
2. The user is currently on the "Settings" page.

## Steps to Reproduce
1. From the Settings menu, navigate into the "Profile" section.
2. Tap the "Back" button to return to the Settings menu.
3. Re-enter the "Profile" section for a second time.
4. Tap the "Back" button again.

## Expected Result
The "Back" button should function consistently every time the user enters the page, successfully returning them to the previous "Settings" menu.

## Actual Result
On the second attempt, the "Back" button becomes completely unresponsive and fails to react to tap gestures. The user becomes soft-locked/stuck on the Profile page, and navigation is completely blocked unless the application is restarted.

