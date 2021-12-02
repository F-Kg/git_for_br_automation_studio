# Getting started

This guide will take you through the first steps in using Git as a version control system for a B&R Automation Studio (AS) project.

## Prerequisites

1. Download and install the most recent version of Automation Studio from the [B&R homepage](https://www.br-automation.com/)
2. Download and install the most recent version of Git from the [Git homepage](https://git-scm.com/)

In this guide, we use Git BASH to use Git from the command line. If you prefer a GUI, the Git homepage has an [overview](https://git-scm.com/download/gui/windows).

## Configure your name and email

If you haven't already entered your name and email in the Git configuration, you must do this now.

Open git bash and enter:

    git config --global user.name '<my_name>'
    git config --global user.email '<my_email@my_domain.com'

![Git config](img/git_config.gif)

## Create a new AS project

![New AS project](img/as_new_project.gif)

## Add a .gitignore file

In your project directory, add a new file and rename it to ".gitignore".

![gitignore](img/gitignore.png)

This file specifies files that you do not want to put under version control, such as binary files and automatically generated files.

Open .gitignore in a text editor and enter:

    /Binaries
    /Diagnosis
    /Temp
    /*.set
    /*.isopen

## Initialize a Git repository

Open git bash in your project directory and enter:

    git init

This creates a Git repository inside your project directory.

![git init](img/git_init.gif)

## Stage your changes

Open git bash in your project directory and enter:

    git add .

This stages all files (except the ones in .gitignore) for your next commit.

![git add](img/git_add.gif)

## Commit

Open git bash in your project directory and enter:

    git commit -m 'initial commit'

![git commit](img/git_commit.gif)

## Conclusion

Congratulations! Your project is now under version control with Git.

But this is just the beginning, there is **much** more to Git! You will probably want to use a remote repository on your server or on a hosted platform like GitHub, so that you have a backup of your data and so that you can work in teams.

In this tutorial, we decided to only show you the very first steps. With the exception of the .gitignore settings, everything in this tutorial is standard Git and not B&R-specific. There are a lot of great ressources out there that cover Git in great depth, here is a small selection:

- [Video tutorial by Mosh](https://www.youtube.com/watch?v=8JJ101D3knE&t=190s)
- [The official git documentation](https://git-scm.com/doc)
