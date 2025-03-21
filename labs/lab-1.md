# Lab 1: Setting Up Git
In this section, we will learn how to install Git, configure your user information (name and email), and set up your first repository. We'll guide you through the initial setup process.

> [!NOTE] 
> ### Before You Begin
> The steps in this lab exercise require a computer. Your computer can be Windows, Linux or macOS. You will be running these steps in the terminal/CLI.  You will not be able to do this on a phone or tablet.

## Video Guides
If you prefer to follow a step-by-step video guide as you take this lab exercise, watch the [Chapter 1 – Lab 1 – Setting Up Git](videos/youtube) video.

## Installing Git
Launch your terminal in **macOS** or **Linux**, or Command Prompt or PowerShell in Windows. 
1. First, check if Git is already installed on your system by opening a terminal or command prompt and typing 
    ```bash
    git –version
    ```
    If Git is installed, you will see the installed version number.
2. If Git is not installed, you can download it from the [official website](https://git-scm.com/downloads) and follow the installation instructions for your operating system.
## Configuring User Identity
3.	After installing Git, you need to configure your user identity by setting your name and email address.
4.	In the terminal or command prompt and type 
    ```bash
    git config --global user.name "Your Name"
    ```
    This command sets the name that will be associated with your Git commits globally on your system. This means that every time you make a commit, Git will use of “Your Name” as the author name. 
5.	Then type
    ```bash
    git config --global user.email "your_email@example.com"
    ```
    This sets the email address that will be associated with your Git commits globally on your system. This means that every time you make a commit, Git will use this email address as the author email. 
## Creating a Local Repository
Before you create a local repository, I would recommend you set aside a separate directory designated as a parent directory for storing your local git repos. Every git repo resides in a separate directory. You may for example want to create the following structure:

<img width="436" alt="git-repo-directory-structure" src="https://github.com/user-attachments/assets/1ee681cc-b605-4f38-8f91-3e543af1eebd">

_Figure 2.6: A sample directory structure with parent directory for storing local repos._

Let's get started, with the following steps:

1.	Skip this step if you already have a desired location. Otherwise, type
    ```bash
    mkdir all_my_repos && cd all_my_repos
    mkdir app1 && cd app1
    ```
2.	To create a new local repository, navigate to the desired location on your computer using the terminal or command prompt. If you are new to the CLI, you can read this article  (https://opensource.com/article/21/8/linux-change-directories) on how to navigate to a directory in the terminal. Type 
    ```bash
    git init
    ```
    This will initialize a new repository and create a new .git directory containing all the necessary files for version control.
    Your repo has now been initialized. Any changes you make to that directory e.g. create a file, modify a file, add a file, delete a file, etc. would be tracked.
3.	Check the status of git by typing
    ```bash
    git status
    ```
    You should get the following result:
  	
    <img width="472" alt="git-repo-no-commits" src="https://github.com/user-attachments/assets/998898cf-69f1-41b3-b4ed-43f615df82c4">
    
    This indicates that your working branch is main and no changes or commits have been detected yet in this repo.
## Creating Your First Application Source Code
5.	In your initialized directory, create a new file (you can also move an existing file into it) by typing
    ```bash
    echo "alert("Hello world")" >> my_new_file.js
    ```
6.	Now check the status of your repo again by typing git status. You should get the following result:

    <img width="473" alt="git-repo-commit-no-staged-file" src="https://github.com/user-attachments/assets/111e1a41-5753-4679-8778-b4f451df204e">

    Here, a new file has been detected but it has not been tracked for versioning yet.
7.	To include the new file in version control so that subsequent changes to it would be tracked, type
    ```bash
    git add "<file>", where <file> is the filename of the new file you added. Then type git status again. You should get the following result:
    ```
    
    <img width="473" alt="git-repo-changes-staged-file" src="https://github.com/user-attachments/assets/019e8ae1-2e3b-4f85-8d1b-d50a80dc1f99">

    The change in this file has now been recognized and the change detected is that it is a new file added. It is now in the staging area, ready for a commit.
8.	To commit the changes in your staging area (you can stage multiple files and commit all at once), you will use the git commit command followed by the -m flag and then your message in quotes. Type
    ```bash
    git commit -m "Adds my first source code file"
    ```
Congratulations! You have completed your first version control exercise. Your source code is in safe hands.




