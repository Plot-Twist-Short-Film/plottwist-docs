# **{{ project.name }} Assets Manager**

!!! help ""
    This is the main tool to manage the different assets available for {{ project.name }} project.
    
    Using this tool you can:
    
    * **Open** Asset Files (model, shading, rig, etc)
    * **Lock** & **Unlock** Asset Files
    * **Synchronize** Asset Files
    
***

## **Kitsu**

![Kitsu Icon](../../img/logos/kitsu.png?style=centerme)


Kitsu is the Production Manager tool that we are using in {{ project.name }}.


!!! important
    {{ project.name }} Assets Manager intensively uses the information stored in {{ project.name }} Kitsu database to show different information of the assets.
    For this reason, is **mandatory** to be connected to the Internet when the tool is launched.
    
***

### **Login into Kitsu**

 > {{ project.name }} Assets Manager - Login into Kitsu
![{{ project.name }} Assets Manager](../../../img/tools/assetsmanager/1.png?style=centerme)

If you launch {{ project.name }} Assets Manager and no Kitsu login information is detected you will have to login into Kitsu.

 > Kitsu Login Toggle button - Not Logged
![Kitsu Login Toggle button](../../../img/tools/assetsmanager/kitsubutton.png?style=centerme)

!!! note
    The first time you launch {{ project.name }} Assets Manager you will need to login into Kitsu.

 > {{ project.name }} Assets Manager - Kitsu Login Dialog
![Kitsu Login Dialog](../../../img/tools/assetsmanager/2.png?style=centerme)

To login into Kitsu, you need to left-click on top ot the **Kitsu Login Toggle** button. This will show **Kitsu Login Dialog** in the center of your screen.

Kitsu Login Dialog has tree fields you can edit:

* **Email**: In this field you need to type the email you used during Kitsu registration.
* **Password**: In this field you need to type the password you used during Kitsu registration.
* **Store Credentials**: If you check this checkbox, your credentials will be store and you won't have to type them again.

Once you are ready, click on **Login** button to continue.

If your login credentials are valid, {{ project.name }} assets info will be loaded.

![{{ project.name }} Assets Manager - Kitsu Login](../../../img/tools/assetsmanager/3.png?style=centerme)

***

## **Main UI**

![{{ project.name }} Assets Manager - Main UI](../../../img/tools/assetsmanager/4.png?style=centerme)

<center>

|          |   Description    |
| -------- |:-------------:|
| ![Red Color](../../img/colors/red.png?style=centerme) | Kitsu Login |
| ![Blue Color](../../img/colors/blue.png?style=centerme) | {{ project.name }} Assets Viewer |
| ![Green Color](../../img/colors/green.png?style=centerme) | {{ project.name }} Asset Info |
| ![Purple Color](../../img/colors/purple.png?style=centerme) | {{ project.name }} Assets Manager Info Status Bar |

</center>

### **Kitsu Login**

In this section you can find de Kitsu Toggle button and also the Logout button.

If you clikk in the **Kitsu Toggle** button a popup with info of you Kitsu user will appear.

 > Kitsu Info
![Kitsu Info](../../../img/tools/assetsmanager/kitsuinfo.png?style=centerme)

If you want to logout from Kitsu you can press the logout buttuon. After doing it, a dialog will ask you if you want
to remove the stored credentials or not.

 > Kitsu Logout
![Kitsu Logout](../../../img/tools/assetsmanager/kitsulogout.png?style=centerme)

***

### **Assets Viewer**

The Assets Viewer is where all {{ project.name }} Assets are loaded. 

#### **Asset**

 > Asset
![Assets Viewer Asset](../../../img/tools/assetsmanager/asset.png?style=centerme)

An Assets Viewer Asset is composed by:

* **Image** that shows how the asset is visually.
* **Name** that shows the name of the asset.

***

##### **Contextual Menu**

 > Asset Contextual Menu
![Asset Contextual Menu](../../../img/tools/assetsmanager/assetcontextmenu.png?style=centerme)

If you **right-click** on top of one of the assets, the **contextual menu** of the asset will appear, showing the following options:

<center>

|    |      Name      |   Description    |
| -------- |:-------------:| :---------:|
| ![Kitsu icon](../../img/icons/kitsu.png?style=centerme) | **Open in Kitsu** | Open Asset Kitsu webpage in your default web browser. |
| ![Artella icon](../../img/icons/artella.png?style=centerme) | **Open in Artella** | Open Asset Artella webpage in your default web browser. |
| ![Eye icon](../../img/icons/eye.png?style=centerme) | **View Locally** | Open local folder where Asset files are located in your computer. |
| ![Synchronize icon](../../img/icons/sync.png?style=centerme) | **Synchronize** | Open asset synchronization options. |

</center>

!!! info "Asset Synchronization Options"

    Here you can find the different types of asset synchronization currently supported:
    
    <center>
    
    |    |      File Type      |   Description    |
    | -------- |:-------------:| :---------:|
    | ![Download icon](../../img/icons/download.png?style=centerme) | **All** | Synchronizes all the files of the asset. |
    | ![Textures icon](../../img/icons/textures.png?style=centerme) | **Textures** | Synchronizes texture files of the asset. |
    | ![Shading icon](../../img/icons/shading.png?style=centerme) | **Shading** | Synchronizes shading files of the asset. |
    | ![Model icon](../../img/icons/model.png?style=centerme) | **Model** | Synchronizes model files of the asset. |
    | ![Rig icon](../../img/icons/rig.png?style=centerme) | **Rig** | Synchronizes rig files of the asset. |
    | ![Groom icon](../../img/icons/groom.png?style=centerme) | **Groom** | Synchronizes groom files of the asset. |
    
    </center>
    
    !!! note
        Take into account that depending of the type asset some files are not available. For example, grooming files are only available for characters.

***

### **Assets Info**

The Assets Info area is where all the properties of the selected Asset are loaded.

To load the information of an asset you just need to left-click an Asset in the Assets Viewer

![Assets Info](../../../img/tools/assetsmanager/6.png?style=centerme)

<center>

|          |   Description    |
| -------- |:-------------:|
| ![Blue Color](../../img/colors/blue.png?style=centerme) | Asset Name |
| ![Red Color](../../img/colors/red.png?style=centerme) | Asset Shortcuts |
| ![Purple Color](../../img/colors/purple.png?style=centerme) | Asset Image  |
| ![Green Color](../../img/colors/green.png?style=centerme) | Asset Status Buttons |
| ![Yellow Color](../../img/colors/yellow.png?style=centerme) | Asset File Shortcuts |
| ![Cyan Color](../../img/colors/cyan.png?style=centerme) | Asset Versions Info |

</center>

#### **Asset Shortcuts**

<center>

|    |      Name      |   Description    |
| -------- |:-------------:| :---------:|
| ![Artella icon](../../img/icons/artella.png?style=centerme) | **Open in Artella** | Open Asset Artella webpage in your default web browser. |
| ![Folder icon](../../img/icons/folder.png?style=centerme) | **Open Local Folder** | Open local folder where Asset files are located in your computer. |

</center>

#### **Asset Status Buttons**


<center>

|    |      Name      |   Description    |
| -------- |:-------------:| :---------:|
| ![Working icon](../../img/icons/working.png?style=centerme) | **Working** | Open Asset Working Files. |
| ![Published icon](../../img/icons/box.png?style=centerme) | **Published** | Open Asset Published Files. |

</center>

#### **Asset File Shortcuts**

<center>

|    |      File Type      |   Description    |
| -------- |:-------------:| :---------:|
| ![Textures icon](../../img/icons/textures.png?style=centerme) | **Textures** | Open folder where textures files are located. |
| ![Shading icon](../../img/icons/shading.png?style=centerme) | **Shading** | Open Shading File. |
| ![Model icon](../../img/icons/model.png?style=centerme) | **Model** | Open Model File. |
| ![Rig icon](../../img/icons/rig.png?style=centerme) | **Rig** | Open Rig File. |
| ![Groom icon](../../img/icons/groom.png?style=centerme) | **Groom** | Open Groom File. |

</center>

!!! tip
    ![Artella icon](../../img/icons/artella.png?style=centerme)
    
    ***
    
    At the right of each Asset File button there is a second button with the Artella Icon. If you press this icon, 
    current versions of the selected file type will be display in the Asset Version Info

</center>

#### **Asset Version Info**


In this section the version tree for the selected asset is displayed

***

### **Info Status Bar**

This bar will show important messages for the users. There are 4 types of message:

<center>

|          |   Description    |
| -------- |:-------------:|
| ![Ok Message](../../img/icons/ok.png?style=centerme) | Message that appears when an operation is **successful** |
| ![Info Message](../../img/icons/info.png?style=centerme) | Message that appears to given **information** to the user |
| ![Warning Message](../../img/icons/warning.png?style=centerme) | Message that appears when a **non critical error** happens |
| ![Error Message](../../img/icons/error.png?style=centerme) | Message that appears when a **critical error** happens |

</center>