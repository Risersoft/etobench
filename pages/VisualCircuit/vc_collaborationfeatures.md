---
title: Collaboration Features
keywords: Collaboration Features
sidebar: viscir_sidebar
permalink: visual-circuit/collaboration-features.html
folder: VisualCircuit
hide_sidebar: false
comments: false
---

# Collaboration Features



VisualCircuit is built with collaboration in mind. Because all data is stored in a common database, it gives both ease and power to teams to work together to create great results.

VisualCircuit does not allow two users to edit the same thing simultaneously. For this purpose, whenever an entity is edited, a lock is acquired on that row before giving access. If another user is already editing, a dialog box such as the following is displayed -

![](/images/collaboration-features.png)

When the user “Boss” finishes editing, the lock is released and now it is free to be edited again. The username is taken from the currently logged on Windows User.

If the machine which acquired the lock crashes or freezes for some reason, the lock is not released until the object is open again from the same machine and then closed.
