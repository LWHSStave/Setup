---
title: Referencing _library_**.jar**
---
# Referencing _library_**.jar**

This page provides instructions for setting up a custom java **.jar** library in VSCode, such that your code can reference its classes.

- [ ] Obtain the _library_**.jar** file. This is typically given to you as part of the various assignment packages. Most commonly, this is [`drawing-lib-2.0-shaded.jar`](https://florinteo.github.io/EduCode/DrawingLib/drawing-lib-2.0-shaded.jar), which is used in multiple assignments such as _AP3.CafeArt_ and _DS2.ColoringBook_.
- [ ] Drop the _library_**.jar** file in your project, if it is not already there, typically in a lib folder. Since initially the library is not configured with java, your code referencing its classes will show multiple errors, as exemplified below:  

    <img alt="RefJar-0" src="https://lwhsstave.github.io/Setup/RefJar/res/RefJar-0.png">

    Notice:  
    - _library_**.jar** shows both in the EXPLORER and in JAVA PROJECTS panes. If this is not the case, right-click on the top node in the JAVA PROJECTS pane (_Workspace_ in the example) and _Configure Classpath_ to lead to your code.
    - _library_**.jar** does **not** show under the *Referenced Libraries* node. This is saying that Java does not know of this file hence its classes are not accessible.
- [ ] Simply drag _library_**.jar** from wherever you have it in your project (_lib_ folder in the example) in the *Referenced Libraries* node.

All going well, the Referenced Libraries should show _library_**.jar** in the list, and your code should clear of any errors:

- [ ] <img alt="RefJar-1" src="https://lwhsstave.github.io/Setup/RefJar/res/RefJar-1.png">
