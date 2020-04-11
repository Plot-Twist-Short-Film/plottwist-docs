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

**Autodesk Maya**: A big part of our pipeline it's oriented to be used inside DCCs. Our core target DCC is Maya but 
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

## **Repositories**

All {{project.name}} repositories are included inside a **[GitHub Organization](https://github.com/Plot-Twist-Short-Film)**.

Also, is important to notice that {{project.name}} pipeline is based on **[ArtellaPipe](https://github.com/ArtellaPipe)**.
This library basically give us a core implementation of different tools to manage Artella based projects. It allow us
to extend already tools or add new tools in an easy way.

!!!info
    You can find more information about **ArtellaPipe** in the following link.
    
So, to start with, you will need to clone all Plot Twist repositories into your local drive. To automatize this process
you will be able to find some scripts in the following repository: **[plottwist-dev-setup](https://github.com/Plot-Twist-Short-Film/plottwist-dev-setup)**.
Just follow the instructions that you will find in the README.rst file.

Once you have all the repositories downloaded you will be able to move them anywhere into your computer. Also, now you 
can, depending on the selected IDE, configure the project and so on.

## **Development Virtual Environment**

During all our development we are going to use a virtual environment for 2 main purposes:

1. If we need to add new package dependencies we can add them very easily to our development environment.
2. Is very easy to add or remove local repositories to that virtual environment, so we can control very precisely 
which repos we are editing and which no.

To setup your development virtual environment for Plot Twist follow the next steps: