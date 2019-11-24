# **How to Save a File?**

When working in {{ project.name }} you can **Save** your DCC scenes (Maya scenes, Houdini scenes, etc) using normal
saving functionality (usually with Ctrl + S shortcut). The problem is that when saving files with this option your files
can store unnecessary data. 

To avoid this, you can use {{ project.name }} Save functionality. For that, you just need to press **{{ project.name }} Save**
button in {{ project.name }} **Main** Shelf.

> {{ project.name }} Save
![{{ project.name }} Save](../../../img/tools/shelf/icons/save.png?style=centerme)

## **What it does?**

1. Delete nodes in the scene that are unknown.
2. Delete Turtle nodes that are unused.
3. Delete nodes from plugins that are not being used or not installed in user machine.
4. Remove generic garbage nodes from Maya.
5. Remove Student License from Maya file (if license is found) 