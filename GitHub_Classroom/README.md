# GitHub Classroom Setup

---
## GitHub Account
You will need a school-approved account at <a href="https://github.com/" target="_blank" rel="noopener">GitHub</a> in order to receive, work on and submit coding assignments. This account needs to comply to the following rules:
- The account handle should be *YourStudentId-LWHS* (i.e. *1234567-LWSD*).
- The email linked to the account should be your @lwsd.org email.
- The profile should have your correct *Name* filled in.
- It should have 2FA enabled, hooked into the Authenticator app on your phone.

If you already have a personal GitHub account which you want to use for school, you can configure it to comply to these rules but the recommendation is to create a new account.

---
## VSCode & Git Setup
With GitHub Classroom you can download an assignment directly in VSCode, such that you can start coding and then submitting it upon completion. For a smooth usage of this capability, the following configuration steps are recommended: 
- [ ] VSCode should be opened on a <u>folder</u> and not a <u>workspace</u>. A workspace is a special configuration file (i.e. *.*code-workspace*), created by VSCode in order to consolidate multiple projects in the same view. In class we used a *Workspace* <u>folder</u>, so you should be good.
- [ ] (Optional): There is a VSCode extension, *Markdown All in One* which you may find useful. It provides a cleaner rendering of the `.md` files. These are text file with minimal formatting capabilities (similar to HTML) which will come with the assignments. It is useful to install this extension from the `Extensions` button from the VSCode left bar.
- [ ] Git configuration should include your **user.name** and **user.email**. This is not done by default so you need to do this once:<br> Open a terminal window in VSCode (menu: `Terminal` > `New Terminal`), then type in the following commands. Provide your name and your @lwsd.org email address in each:
```
    > git config --global user.name "Your Name"
    > git config --global user.email Your@email
```
---
## GitHub Classroom Assignment
With your GitHub account created and your VSCode & Git configured, the following steps show how to receive and download an assignment, work on it and finally submitting it, all from within VSCode.
   
1) <b>Get the assignment</b><br>You will receive the assignment as a web link, communicated via some channel (i.e. posted in Canvas). For this example we'll use a simple "dummy" assignment, one for each Period: <a href="https://classroom.github.com/a/rdbLaS3r" target="_blank" rel="noopener">U0.Hello (Period_1)</a> and <a href="https://classroom.github.com/a/MC8hoQwh" target="_blank" rel="noopener">U0.Hello (Period_2)</a>.

2) <b>Create your assignment repo in the GitHub Classroom</b><br>Click on the link corresponding to your period. A web page opens, reading "Join the classroom..." and containing an *Identifiers*. list. Find your name in the list and click `Accept this assignment`. You get to a page reading *"You're ready to go!"* and showing an <u>assignment repository</u> (or repo) link underneath. <span style="color: red;">Copy that link in clipboard</span>. If you miss it, you can still locate it from within your GitHub account:
	- [ ] Log in your *YourStudentID_LWSD* GitHub account.
	- [ ] Go to your *Profile* / *Organizations* / *LWHSStave* / *Repositories* and locate the repository that was created for you for the given assignment. It'll look something like *u0-hello-world-YourStudentId-LWSD*.
	- [ ] Click the `<> Code` button to copy the reposity link into Clipboard.

3) <b>Download the assignment repo to your PC</b><br>Once you have the <u>assignment repository</u> in clipboard, open VSCode and clone it on your computer:
	- [ ] In the VSCode search bar (on the title bar) type `> clone` then, from the drop down list, select `Git: Clone`.
	- [ ] Paste the repo link in the edit box that pops up.
	- [ ] In the file selection dialog that opens, <span style="color: red">navigate to your *Workspace* folder</span> then click `Select as Repository Destination`.
	- [ ] A popup shows up asking: "Would you like to open the cloned repository...", giving four options: `Open`, `Open in New Window`, `Add to Workspace` and `Cancel`. Choose <span style="color: red">Cancel</span>!!.  

    You'll notice an *assignment* folder showing up in your *Workspace* folder, containing all the files necessary for the assignment. 

4) <b>Add assignment folder to Java Classpath</b><br>Since the assignments contain or ask you to write Java code, we need to add the assignment folder to the Classpath, such that Java can locate the code properly:
    - [ ] In the VSCode search bar (on the title bar) type `> classpath` then, from the drop down list, select `Java: Configure Classpath`.
    - [ ] In the Source Paths, you might see only one entry, listing the `.` folder. Click on the `+ Add Source Root...` then navigate to the assignment folder.
    - [ ] Scroll down on that page to locate and click the `Apply Settings` button, then close the `Project Settings` page.
  
    The folders added to Java Classpath are driving the way Java locates your code, and works in conjunction with the `package` declarations at the beginning of each .java file.

5) <b>Working on the assignment</b><br>You are now ready to work on the assignment:
    - [ ] Inspect the README.md file. It is written in an HTML-like language. You can see it rendered more comfortably if you click on the preview button from the top-right corner of its window.
    - [ ] Inspect the `HelloWorld.java` file and make the changes requested by the assignment
    - [ ] Execute your program and copy/paste its output at the end of the README.md file.

6) <b>Submitting the assignment</b><br>All changes made and files saved, you should notice a badge (blue bubble) marking the `Source Control` button on the buttons left bar in VSCode. It indicates the files that had changed since the "last-known-good" state of the code, which in our case is the moment we downloaded the repo.
    - [ ] Click on the `Source Control` button. You'll notice the two files modified for this assignment, `HelloWorld.java` and `README.md` listed in the *Changes* section.
    - [ ] Hover over the *Changes* section and notice a `+` sign appearing. Click on it. This results in the two files being moved under the *Staged Changes* section.
    - [ ] Notice right above the `Commit` button a *Message* edit field. Type in a custom message, indicating the nature of this change. I.e: "Assignment complete!". Then click the `Commit` button.
    - [ ] Notice the button now reading `Sync Changes`. Click on it to finally upload your work into the GitHub Classroom.

Your work is now DONE! The teacher has access to your work, can clone it and provide feedback directly on your code. We'll learn later how to receive and review this feedback.
