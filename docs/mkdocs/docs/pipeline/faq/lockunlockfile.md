# **Locking & Unlocking Files in Artella**

Artella uses a lock/unlock system to allow artists to make sure that the file they're working on right now is not 
modified by other user.

## **Lock & Unlock Workflow**

**Lock/Unlock** workflow is explained in the following diagram:

> Artella Lock/Unlock Workflow
![Artella Lock/Unlock Workflow](../../../img/faq/diagrams/lockunlock.png?style=centerme)

As you can see in the diagram, Artella lock/unlock system is composed by **2 steps**:

1. When you want to work on a file, before starting to work on it you need to **LOCK** it. Doing this, you make sure that **no other artist can edit that file** while your are working on it.
2. At this point you have **2 options**:
    1. You are not happy with your changes and you want to **"recover"** the file to the **initial state** of the file when you started to work with it. To do this, just **UNLOCK** the file. 
    2. You hare happy with your changes in you want to **submit them to Artella**. Just upload your changes to Artella server **(New Version)** and after that **UNLOCK** your file. Your changes won't be deleted because they are already stored in Artella server.
    
    
!!! warning
    Before unlocking a file, make sure that your changes are loaded into Artella (you need to create a new version
    of the file for that). Otherwise, your changes will be lost after the unlocking process.

***
    
## **Lock & Unlock in {{ project.name }}**

When working in {{ project.name }} you have **3 different ways** to unlock & unlock files.


### **{{ project.name }} Artella Manager**        

???+ example "Artella Manager"

    !!! info
        Using Artella Manager you can navigate easily through the files located in your local drive or the files +
        located in Artella server and lock/unlock files without the need of going to Artella webpage to find the file
        you want to lock or unlock.
        
        Also you can lock or unlock a file by giving the specific URL where the file is located in Artella server.
        
    > Open {{ project.name }} Artella Manager Tool
    ![Artella Manager 1](../../../img/faq/lockunlock/manager_1.png?style=centerme)
    
    ***
    
    > In Artella Manager Tool, make sure that you have Local tab opened and search the file you want to lock
    in the folders tree. This tree shows all the files of {{ project.name }} project that you have synced in your
    computer. Once you have the file, select it by pressing Left-Click on top of it.
    ![Artella Manager 2](../../../img/faq/lockunlock/manager_2.png?style=centerme)

    ***
    
    > Open item contextual menu by pressing Right-click on top of it.
    ![Artella Manager 3](../../../img/faq/lockunlock/manager_3.png?style=centerme)
    
    ***
    
    > Press **Lock File** button to lock the file
    ![Artella Manager 4](../../../img/faq/lockunlock/manager_4.png?style=centerme)
    
    ***
   
    > Press **Unlock File** button to unlock the file
    ![Artella Manager 5](../../../img/faq/lockunlock/manager_5.png?style=centerme)
    
***

### **{{ project.name }} Artella Uploader**        

???+ example "Artella Uploader"

    !!! info
        Using Artella Uploader you can lock or unlock multiple multiples files located in a given path
        
    > Open {{ project.name }} Artella Uploader Tool
    ![Artella Uploader 1](../../../img/faq/lockunlock/uploader_1.png?style=centerme)
    
    ***
    
    > Left click on Select Path button
    ![Artella Uploader 2](../../../img/faq/lockunlock/uploader_2.png?style=centerme)

    ***
    
    > Select root folder. All files located in this folder and its subfolders will be loaded in the files list
    ![Artella Uploader 3](../../../img/faq/lockunlock/uploader_3.png?style=centerme)
    
    ***
    
    > After selecting the folder all the files will be loaded in the files list and the current version of the files
    in your Artella server will be checked. Wait until the process is complete.
    ![Artella Uploader 4](../../../img/faq/lockunlock/uploader_4.png?style=centerme)
    
    ***
    
    > Make sure that only the items you want to lock are checked. By default, all items are checked. After that, press
    the **Lock** button
    ![Artella Uploader 5](../../../img/faq/lockunlock/uploader_5.png?style=centerme)
    
    ***
    
    > Follow same steps and press **Unlock** button, to unlock items
    ![Artella Uploader 6](../../../img/faq/lockunlock/uploader_6.png?style=centerme)

***    

### **{{ project.name }} Lock & Unlock Shortcuts**

???+ example "Lock & Unlock"
    
    !!! info
        This method is useful to lock and unlock files that are currently opened in your DCC (Maya, Houdini, etc).
    
    > Open the file you want to edit in your DCC (we use Maya in this example)
    ![Lock/Unlock 1](../../../img/faq/lockunlock/lockunlock_1.png?style=centerme)
    
    ***
    
    > After doing your changes (and after saving your Maya scene), you just need to press **Lock** button located
    in {{ project.name }} **Main** shelf.
    ![Lock/Unlock 2](../../../img/faq/lockunlock/lockunlock_2.png?style=centerme)
    ![{{ project.name }} Save](../../../img/tools/shelf/icons/lock_file.png?style=centerme)
    
    !!! info
        In Windows, after locking the file a tray message will appear in the bottom right corner of your screen
        ***
        ![Lock/Unlock 3](../../../img/faq/lockunlock/lockunlock_3.png?style=centerme)

    !!! tip
        You can check if your file is has been locked successfully by pressing **Check Lock/Unlock** button located
        in {{ project.name }} **Main** shelf.
        ![Lock/Unlock 4](../../../img/faq/lockunlock/lockunlock_4.png?style=centerme)
        ![{{ project.name }} Check Lock/Unlock](../../../img/tools/shelf/icons/lock_check.png?style=centerme)
            
        If you have the file locked the following message will appear in top area of Maya viewport:
        ![Lock/Unlock 5](../../../img/faq/lockunlock/lockunlock_5.png?style=centerme)
        
        Otherwise, following message will appear if the file is not locked by anyone:
        ![Lock/Unlock 6](../../../img/faq/lockunlock/lockunlock_6.png?style=centerme)

    ***
    
    > To unlock the file, you just need to press **Unlock** button located in {{ project.name }} **Main** shelf.
    ![Lock/Unlock 7](../../../img/faq/lockunlock/lockunlock_7.png?style=centerme)
    ![{{ project.name }} Unlock](../../../img/tools/shelf/icons/unlock_file.png?style=centerme)
    
    !!! info
        In Windows, after unlocking the file a tray message will appear in the bottom right corner of your screen
        ***
        ![Lock/Unlock 9](../../../img/faq/lockunlock/lockunlock_9.png?style=centerme)
    
    ***
    
    > Afer pressing Unlock button a popup window will appear, warning you that if you unlock a file without upload a new 
    version of it to Artella server, all the changes done to that file will be lost. Press Ok, if you are happy with it.
    ![Lock/Unlock 8](../../../img/faq/lockunlock/lockunlock_8.png?style=centerme)
    
    !!! info
        To learn how to Submit new versions of a file to Artella server just follow stpe explained in this section: 
        **[How to upload new version?](../newversion)** 

***

### **Artella webpage**

???+ example "Artella Webpage"
    
    !!! info
        This is the usual way that Artella has to lock/unlock files. It's not a bad option at all but you will need to 
        manually find the asset file you want to lock in Artella server and lock/unlock it manually.
    
    > Open your favorite web browser and browse to the Artella page where the file you want to lock/unlock is located.
    ![Artella 1](../../../img/faq/lockunlock/artella_1.png?style=centerme)
    
    ***
    
    > Right-click on top of the item to open item contextual menu. In this menu you just need to check **Edit Mode** checkbox
    ![Artella 2](../../../img/faq/lockunlock/artella_2.png?style=centerme)

    !!! tip
        Sometimes, checking **Edit Mode** fails, so you will need to try to check multiple times.
    
    ***
    
    > After locking the file, you can check that file is locked because your image will appear in the top left border of the file icon
    ![Artella 3](../../../img/faq/lockunlock/artella_3.png?style=centerme)
    
    ***
    
    After doing your changes (and after saving your Maya scene), if you are not happy with your changes you just need
    to:
    
    > Right-click on top of the item to open item contextual menu. In this menu you just need to check **Edit Mode** checkbox
    ![Artella 4](../../../img/faq/lockunlock/artella_4.png?style=centerme)
    
    > A Revert window will appear, this window will warn you about the fact that you are going to **revert** your changes. This
    means that the changes you have done will be delete and the file will be restored with the state of the file before you edited it.
    Press Revert button to do unlock the file or Cancel to stop the unlock process.
    ![Artella 5](../../../img/faq/lockunlock/artella_5.png?style=centerme)
    
    ***
    
    Otherwise, if you are happy with your changes, you just need to upload your changes into Artella server. You can 
    do it following steps explained in: **[How to upload new version?](../newversion)** 
    
    ***
    
    After creating a new version, you just need to:
    
    > Open contextual menu and uncheck Edit Mode checkbox
    ![Artella 8](../../../img/faq/lockunlock/artella_8.png?style=centerme)
    
    Your new version is uploaded and your file is unlocked so other users can edit it if necessary.
    
    !!! info
        Notice that in Artella you MUST to unlock the file manually after creating a new version. Using {{ project.name }}
        tools, the unlock operation can be done automatically.

