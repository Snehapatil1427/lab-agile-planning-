---
name: User Story
about: 'this is user story issue template '
title: ''
labels: ''
assignees: ''

---

As a registered customer  
I need the ability to reset my password  
So that I can regain access to my account if I forget it  

* A "Forgot Password" link is available on the login page  
* Password reset link will be valid for 24 hours  
* Reset link will be sent to the customer’s registered email address  

### Acceptance Criteria

```gherkin
Given I am on the login page
When I click the "Forgot Password" link
Then I should be prompted to enter my registered email address

Given I enter a valid registered email address
When I submit the form
Then I should receive a password reset email

Given I click the link in the email within 24 hours
When I set a new password
Then my account should be updated and I should be able to log in with the new password
```
