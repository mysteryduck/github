# GitHub tutorial (for RStudio)

## Contents

* [Setup Git on RStudio](#setup-git-on-rstudio)
* [Create a new GitHub repository](#create-a-new-github-repository)
* [Create a new RStudio project](#create-a-new-rstudio-project)
* [Useful resources](#useful-resources)



## Setup Git on RStudio

In RStudio, click on the 
**RStudio** menu bar and go to **Preferences**

<img src="https://github.com/mysteryduck/github/blob/master/img/0-1.png" height="200">

Go down to the **GIT/SVN** tab and ensure **Enable version control interface for RStudio projects** is checked.
 
Note that clicking on the **Using Version Control with RStudio** link will take 
you to a site that describes how to set up Git and lists some excellent 
resources to help you learn more about Git. Ignore this for now. 

Instead, we're now going to encrypt communication between our laptops and GitHub. 
To do this we need to generate a certificate. Click on **Create RSA Key...**

<img src="https://github.com/mysteryduck/github/blob/master/img/0-2.png" height="500">

Now, click **Create** to generate your RSA key

<img src="https://github.com/mysteryduck/github/blob/master/img/0-3.png" height="500">

It should look like this

<img src="https://github.com/mysteryduck/github/blob/master/img/0-4.png" height="500">

Now you need to copy your public key and register it with GitHub. Click on **View public key**

<img src="https://github.com/mysteryduck/github/blob/master/img/0-5.png" height="500">

Copy the key to your clipboard

<img src="https://github.com/mysteryduck/github/blob/master/img/0-6.png" height="500">

Then in GitHub, in your **Personal settings**, open the **SSH and GPG keys** tab 

<img src="https://github.com/mysteryduck/github/blob/master/img/0-7.png" height="500">

Create a **New SSH key**

<img src="https://github.com/mysteryduck/github/blob/master/img/0-8.png" height="500">

Paste the public key that you copied from RStudio into the box and click
**Add SSH key** 

<img src="https://github.com/mysteryduck/github/blob/master/img/0-9.png" height="500">

Now back in RStudio, tell Git your user name and email address (these are used 
to label each commit to GitHub). Make sure the email address you enter here is the
same as the one you registered on GitHub.

```{r}
install(usethis)
library(usethis)

use_git_config(
  scope = "user",
  user.name = "insert_github_username_here",
  user.email = "insert_email_address_here"
)
```

RStudio will now remember your details, so don't worry about having to enter 
them again in the future. You should, however, check that your username and 
email address was entered correctly!

```{r}
system("git config --global --list")
```



## Create a new GitHub repository

It's important that you use version control in your project workflow, so let's 
set up a new GitHub repository (you should make a new repository for each
project you're working on). To do this, click **New**

<img src="https://github.com/mysteryduck/github/blob/master/img/1-1.png" height="500">

Choose a short, descriptive name for your repository, and remember to 
generate a README file

<img src="https://github.com/mysteryduck/github/blob/master/img/1-2.png" height="500">

Now **copy** the URL associated with your GitHub repository to your clipboard

<img src="https://github.com/mysteryduck/github/blob/master/img/1-3.png" height="500">



## Create a new RStudio project

In RStudio, click **File** > **New project...**

<img src="https://github.com/mysteryduck/github/blob/master/img/2-1.png" height="300">

Since we're integrating version control into this project workflow, click **Version Control**

<img src="https://github.com/mysteryduck/github/blob/master/img/2-2.png" height="500">

Select the option to clone a project from a **Git** repository

<img src="https://github.com/mysteryduck/github/blob/master/img/2-3.png" height="500">

Now, **paste** your **Repository URL** into the first box and find somewhere to 
store your work. This folder will mirror the contents of your Git repository. 
Click **Browse...** and navigate to the git folder on your desktop. If
you don't have a git folder on your desktop then make one, as it's good 
practice to keep all of your projects together and organised.

<img src="https://github.com/mysteryduck/github/blob/master/img/2-4.png" height="500">





## Useful resources

* https://learngitbranching.js.org

