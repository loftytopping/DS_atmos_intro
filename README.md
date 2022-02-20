# UK_CP
Short course on Clustering and Autoencoders.

This repository contains a small collection of [Jupyter](https://jupyter.org) notebooks designed to practice developing and applying machine learning as part of thr UK COP programme. There are so many courses now available to pick up core operations in Python, this course is targetted more at diving straight in and providing templates for common operations. 

# Table of contents
1. [Course overview](#Course-overview)
2. [Running the models](#Running)
     * 2a. [Using your own machine](#own)
     * 2b. [Using Binder](#Binder)
     * 2c. [Using Google Colab](#Colab)

## Course overview<a name="Course-overview"></a>

This short course has been developed with the notion that a very good way of learning how to apply common machine learning techniques is to dive straight in and tackle a range of examples. In each notebook there are a set of common Python operations. If this is your first time working with Python, you may find it useful to first cover some of the basics.

## Running the models<a name="Running"></a>

If you have not used a Jupyter notebook before, I would reccomend checking out the official [webpage](https://jupyter.org/). There is also information provided in the lectures associated with this course. There are multiple ways you can interact with a Jupyter notebook. The most flexible way is to open and interact with them on your own computer or via a Jupyter-hub instance. However, you can also start an instance of every notebook running in the cloud. We provide details below.

### 2(a). Using your own machine<a name="own"></a>

Having a Python distribution on your own machine is attractive for a number of reasons, not least gaining familiarity with building projects in your own time. If you havent already, I would reccomend installing the Anaconda distribution. You can download a copy using [this link](https://www.anaconda.com/products/individual). That page will give you the option to download a version for Windows, Mac or Linux. Download the graphical installer and, typically, accept all options. Once you have installed this, now open a terminal. On Windows, go to the menu of options and find 'Anaconda Prompt' under the Anaconda folder. On a Mac, go to Finder -> Utilities -> Terminal. If on a Mac, when in this terminal when you type:

> Python

Do you see the reference to Anaconda? For example, you may see something *similar* to:

> Python 3.7.6 (default, Jan  8 2020, 20:23:39) [MSC v.1916 64 bit (AMD64)] :: Anaconda, Inc. on win32

Now we are going to create a virtual environment to run our notebooks in. Virtal environments are a great way of maintaining a 'work space' that is seperate to your default installation. For example, if you are going to start installing lots of bespoke modules, you may sometimes come across a clash of version numbers which then becomes tricky to maintain. In the worst case scenario, this would require a re-installation of Python. So lets create a virtual environment for our project. You can switch-on and switch-ff these virtual environments from the command line/terminal whenever you need them.

If you are on Windows, go back to the Anaconda prompt. If you are on a Mac or Linux, go back to ther terminal. First we need to clone this repository. We should use Git for this, becuase with Git you can keep pulling updates from this repository. If you do not already have Git installed on your machine, you can get it from the [download page](https://git-scm.com/downloads). Once you have installed this, at the prompt/terminal type:

> git clone https://github.com/atmosdave/UK_CP.git

This will download the project to the location you are in already. You can change this location before running the above command, or move the folder later. Github also gives you the option to download a ZIP file of the entire project if you cannot, or do not want, to use Git. Once you have the project downloaded, open a command prompt/terminal and navigate to the project folder. We are now going to use the file 'environment.yml' to create a new virtual environment. Run the following command:

> conda env create -f environment.yml

You will see a number of packages being downloaded by the conda package manager which is part of the Anaconda distribution. Accept any requests and, when finished, you will see a message that resembles the following:

    To activate this environment, use
    
        $ conda activate UK_CP
    
    To deactivate an active environment, use
    
        $ conda deactivate
        
These are the commands for switching on/off this new virtual environment. Let's switch it on. Type the following in the command prompt/terminal:

> conda activate UK_CP

In the command prompt, you will see the name (UK_CP) replace (base). Now we can start an interactive Jupyer notebook session. Still within the project folder, type the following:

> jupyter notebook

Can you see the project folders and files? You are good to go! Every time you now want to open the notebooks for this project, open either the Anaconda prompt or Terminal, activate the environment and then run the last command from within the project folder.

PLEASE NOTE: All of the examples we run in the second notebook would benefit from using a GPU. For this, you can run the examples on Google Colab.

### 2(c). Binder <a name="Binder"></a>

If you do not, or cannot, run Python from your own machine we have provided the ability for you to interact with these files using Binder. The Binder project offers an easy place to share computing environments to everyone. It allows users to specify custom environments and share them with a [single link](https://jupyter.org/binder). Indeed, if you click the link below this will spin-up an individual session for you. Please bare in mind it can take a while to start, and if idle for a short period these sessions will stop. However you can download your notebook file during the session. Everytime you start a Binder link, it will start from scratch.

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/loftytopping/DEES_programming_course/HEAD)

### 2(d). Using Google Colab<a name="Colab"></a>

Google's Colab [Co-laboratory](https://colab.research.google.com) is a great platform for developing machine learning and data-science driven applications on the web. It provides access to free GPU resource (Graphics Processing Units). However it also allows us to run Jupyter notebooks from a Github repository *if you have a Google account*. If you can register or have an existing Google account, using Google Colab is a really nice experience. It will allow you to save individual files and projects to your Google Drive. We dont cover that here. By clicking on the above link it will take you to a page that presents you with options to load existing files from either your Google Drive or from public repositories. However we can also provide you with a clickable link for running individual notebook files, much like Binder. These are given below and are linked to each notebook file. You will likely find these load much quicker than using Binder. However, you may find any images used in the notebook file that are in the Github repo do not load..but not a huge problem. The links to current notebook files are given below. Please note that if you decide to try and run the assessment options in Google Colab you will need to replicate the steps to install Cartopy [if needed] and also load the relevant data files specifically for Colab. Search for those commands in the practical notebooks and ask if you have any questions:

#### Practical 1 
- [![Open notebook In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/atmosdave/UK_CP/blob/master/Notebook_1.ipynb)
  - Solution notebook: [![Open notebook In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/atmosdave/UK_CP/blob/master/solutions/Notebook_1.ipynb)
#### Practical 2 
- [![Open notebook In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/atmosdave/UK_CP/blob/master/Notebook_2.ipynb)
  - Solution notebook: [![Open notebook In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/atmosdave/UK_CP/blob/master/solutions/Notebook_2.ipynb)
