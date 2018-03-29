---
layout: post
title:  "Managing Our Remote Repositories"
date:   2018-03-27 12:00:00 -0400
categories: Git Basics
---

Managing remote repositories can include adding remote repositories, removing remotes that are no longer valid, managing various remote branches and defining them as being tracked or not among an array of many other valuable skills.

What does "Remote" even mean?

Lets decode and clear up what it means for something to be remote. If we break it down to its simplest explanation,
to be remote is just to be elsewhere. It is within reason to think of something that is remote as existing somewhere else on the network/Internet.  However, this doesn't always have to be the case. We could be working on a remote branch that resides on our host machine.

<h2>Git Commands</h2>

In order to see a list of the remote servers that we have configured we use  `git remote`. The server which you clone from is labeled and known as `origin` . Personally, I find this nomenclature easier for remembering which is my original branch. If you are collaborating on a project, or just happen to have more than one remote, the command `git remote -v` will list out all of the remotes and the URLs that Git has associated with them to read and write.

To add a new remote Git repository we can run `git remote add <shortname> <url>`. To fetch the information from another collaborator that is not yet on our repository you can run `git fetch <remote>`.  Running the `git fetch` command, however, will only download the data to your local repository, but in order to merge it to what you are currently working on will require a manual merge. The `git pull` command will automatically fetch and merge the remote branch into your currently working brancy. 

