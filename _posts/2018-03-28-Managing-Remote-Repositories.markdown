---
layout: post
title:  "Managing Our Git Repositories"
date:   2018-03-27 12:00:00 -0400
categories: Git Basics
---

Managing remote repositories can include adding remote repositories, removing remotes that are no longer valid, managing various remote branches and defining them as being tracked or not, among an array of many other skills.

What does "Remote" even mean?

First of all, what does it even mean for something to be remote? Lets decode and clear up what it means for something to be remote. If we break it down to its simplest explanation, to be remote is just to be elsewhere. It is within reason to think of something that is remote as existing somewhere else on the network/Internet.  However, this doesn't always have to be the case. We could be working on a remote branch that resides on our host machine.

<h2>Some Git Basics C</h2>

When we want to create a new repository on our host machine, we will navigate to our desired location in the terminal and run the `git init` command.  This will initialize a git repository in the folder.  From here, we can create new files for our project using our preferred text editor or through the terminal using the `touch` command.  Once we have created our project files, the `git status` command will show us what files git knows exist and color coded red or green depending on their status. 

In order to see a list of the remote servers that we have configured we use  `git remote`. The server which you clone from is labeled and known as `origin` . Personally, I find this nomenclature easier for remembering which is my original branch. If you are collaborating on a project, or just happen to have more than one remote, the command `git remote -v` will list out all of the remotes and the URLs that Git has associated with them to read and write.

To add a new remote Git repository we can run `git remote add <shortname> <url>`. To fetch the information from another collaborator that is not yet on our repository you can run `git fetch <remote>`.  Running the `git fetch` command, however, will only download the data to your local repository, but in order to merge it to what you are currently working on will require a manual merge. The `git pull` command will automatically fetch and merge the remote branch into your currently working brancy.

Once we have sharable project and want to push it upstream we use the command `git push <remote name> <branch name>`. For example, pushing your master to your origin branch would be  `git push origin master`. However, and this is something that i have run into many times in the past, pushing will only work if someone else has not pushed to the clone. If it is the case that you attempt to push after someone else, you will receive a rejection. You will have to fetch and merge the other persons work first.

