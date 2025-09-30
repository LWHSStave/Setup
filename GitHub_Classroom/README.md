# GitHub Classroom Setup

---
## GitHub
You will need a school-approved account at <a href="https://github.com/" target="_blank" rel="noopener">GitHub</a> which needs to comply to the following rules:
- The account handle should be *YourStudentId-LWHS* (i.e. *1234567-LWSD*).
- The email linked to the account should be your @lwsd.org email.
- The profile should have your correct *Name* filled in.
- It should have 2FA enabled, hooked into the Authenticator app on your phone.

If you already have a personal GitHub account which you want to use for school, you can configure it to comply to these rules but the recommendation is to create a new account.

---
## VSCode
- [ ] Check initial VSCode structure (should be opened in some *WorkFolder*, not  workspace).
- [ ] Configure **user.name** and **user.email** in git 
```
    > git config --global user.name "Your Name"
    > git config --global user.email Your@email
```
---
## GitHub Classroom
- [ ] Go to the assignment link corresponding to your period: <a href="https://classroom.github.com/a/rdbLaS3r" target="_blank" rel="noopener">Period_1</a> or <a href="https://classroom.github.com/a/MC8hoQwh" target="_blank" rel="noopener">Period_2</a>. Find your name in the *Identifiers* list and click {*Accept this assignment*}. You get to a page reading *"You're ready to go!"* and showing a repository link underneath. Copy that link in clipboard. If you miss that and close the browser, you can still locate it from within your GitHub account:
	- [ ] Log in your *YourStudentID_LWSD* GitHub account.
	- [ ] Go to your *Profile* / *Organizations* / *LWHSStave* / *Repositories* and locate the repository that was created for you for the given assignment.<br>It'll look something like *u0-hello-world-YourStudentId-LWSD*.
	- [ ] Click the `<> Code` button to copy the reposity link.
- [ ] Open VSCode and clone the assignment repo:
	- [ ] In the search bar from the top type `> clone` then, from the drop down list click select `Git: Clone`.
	- [ ] Paste the repository link in the edit box that pops up.
	- [ ] In the file selection dialog that opens, navigate to the "Workspace" folder you've been using so far for all your code, then click `Select as Repository Destination`.
