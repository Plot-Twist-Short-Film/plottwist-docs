# **Development Setup**

## **Core software**

To develop new tools and scripts for {{project.name}} project you will need at least the following software:

* **Windows 10**: At the long term Plot Twist pipeline should work both in Windows and Mac but our current development
environment is Windows. Since all our code is written using Python we should not have problems to use it in a Mac
environment.

* **Python IDE**: My recommendation would to use **[PyCharm](https://www.jetbrains.com/es-es/pycharm/)** 
because it incorporates really powerful features for searching code and debugging Maya code with it is really easy. 
Also another good option would be to use **[Visual Studio Code](https://code.visualstudio.com/)**. 
If you have another preferred choice you can use it, of course.

* **Repository Management Tool**: {{project.name}} Twist pipeline is very modular, due to this factor we will need to manage
quite a lot of repositories. For this reason we need to make sure that we use a proper tool for manage all those
repositories. My recommendation would be **[GitKraken](https://www.gitkraken.com/b)**, 
**[SourceTree](https://www.sourcetreeapp.com/)** or**[GitHub Desktop](https://desktop.github.com/)**. 
If you have another preferred choice you can use it, of course.

* **Autodesk Maya**: A big part of our pipeline it's oriented to be used inside DCCs. Our core target DCC is Maya but 
currently our pipeline supports different DCCs such as Houdini or Nuke. Depending of the department you are going to 
work with you will need to download more or less DCCs. The only that is mandatory for all departments is Maya.

* **[Python 2.7.16](https://www.python.org/ftp/python/2.7.16/python-2.7.16.amd64.msi)**: We are using this version of 
Python as our core version. Install it in your machine and make sure that you add it in Window system path.

* **[virtualenv](https://virtualenv.pypa.io/en/latest/)** Python library**: A big part of our workflow depends on 
creating virtual environment when necessary. To do that, we use virtualenv Python library. To install just launch 
the following command:

```console
pip install virtualenv
```

## **Setup**

All {{project.name}} repositories are included inside a **[GitHub Organization](https://github.com/Plot-Twist-Short-Film)**.

Also, is important to notice that {{project.name}} pipeline is based on **[ArtellaPipe](https://github.com/ArtellaPipe)**.
This library basically give us a core implementation of different tools to manage Artella based projects. It allow us
to extend already tools or add new tools in an easy way.

!!!info
    You can find more information about **ArtellaPipe** in the following **[link](../artellapipe)** .
    
To setup our {{project.name}} development environment we will need to:

1. Clone all Plot Twist repositories and also ArtellaPipe ones (optional).
2. Setup Plot Twist development virtual environment with proper requirements.

To do this setup, please go to the following repository:  **[plottwist-dev-setup](https://github.com/Plot-Twist-Short-Film/plottwist-dev-setup)** 
and follow the instructions that you will find in the README.rst file.