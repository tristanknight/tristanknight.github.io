<!--
.. title: What I learned from using Git as a version control system
.. slug: first-post
.. date: 2020-02-05 10:45:52 UTC+01:00
.. tags: 
.. category: 
.. link: 
.. description: 
.. type: text
-->

I've recently been learning how to use Git, and I can now see why it is such a popular version
control system. 

#### What is Git and why is version control essential for programmers?
When working on a large project,
some type of version control system is essential -- one needs to be able to keep track of a project's changes and revert to 
a previous version if something goes wrong. Git also assists teams in coordinating work on a project, since it
gives each programmer access to a repository containing the full history of the project's codebase. In addition to simple version control, 
Git provides a multitude of features that improve developers' organization
and productivity. 

#### How does Git work?

After installing and configuring Git, you can easily create a new repository by running the "git init" shell
command in your project's directory. 

A Git repository has three key areas:
   * The Working Directory, which contains the files you can view and edit on your computer 
   
   * The Staging Index, which contains files from the working directory which have been added to the staging 
    index by the user but have not yet been committed
    
   * The Repository, where commits are stored
    

#### What are some of Git's key features?

For a thorough explanation of Git's features, see the [official 
Git documentation](https://git-scm.com/doc). However, I have included a sample of Git's key features, 
which give you the ability to do the following: 

* Add changes to the staging index, and commit stages from the staging 
index to the repository with the "git add" and "git commit" commands.
 You can also remove or edit previous commits. 
 
* Quickly check the commit history with the "git log" command.

* Select which files you'd like Git to ignore 

* Add a tag (such as a version number) to a particular commit with the "git tag" command.

* Maintain parallel sets of changes with Git's branching functionality. Git's branching feature is key 
in allowing large teams of developers to work on multiple features of a project simultaneously. 

* The ability to merge independent branches together. Git will also let the user know if there is a merge conflict 
(i.e. if the branches contain conflicting lines of code), which the will then need to resolve manually.



