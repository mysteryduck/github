# GitHub tutorial (for RStudio)

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



## Setup Git on RStudio







Create a new GitHub repository

<img src="https://github.com/mysteryduck/github/blob/master/img/1-1.png" height="500">

Choose a short, descriptive name for your project, and initialise the project 
with a README file

<img src="https://github.com/mysteryduck/github/blob/master/img/1-2.png" height="500">

Now copy and paste the URL associated with your GitHub repository

<img src="https://github.com/mysteryduck/github/blob/master/img/1-3.png" height="500">

In RStudio, create a new project

<img src="https://github.com/mysteryduck/github/blob/master/img/2-1.png" height="200">

Make sure your new project includes version control

<img src="https://github.com/mysteryduck/github/blob/master/img/2-2.png" height="500">

Select the option to clone a project from a GitHub repository

<img src="https://github.com/mysteryduck/github/blob/master/img/2-3.png" height="500">

Copy and paste your GitHub repository URL into the first box

<img src="https://github.com/mysteryduck/github/blob/master/img/2-4.png" height="500">





Useful resources:

* https://learngitbranching.js.org

