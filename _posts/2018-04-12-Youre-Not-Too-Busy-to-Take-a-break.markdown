---
layout: post
title:  "You're Not Too Busy to Take a Break"
date:   2018-04-12 12:00:00 -0400
categories: 
---

It might seem that your to-do list never ceases to grow. So much so, that you can't possibly find the time to stop your work even for 5 or 10 minutes for something as pointless as a break. Not so fast, though. It's important to not simply go about your day as usual, especially when you know theres a better way of doing something. Allocating time for breaks will in the long run make you happier, increase your focus, lead to better productivity and make you a better worker.  The alternative can have damaging effects on your productivity and mental state.

<h2>Reasons to Prioritize Breaks</h2>

<ol>
    <li>Breaks keep people from getting bored, distracted, tired, and unfocused.</li></br>
    
    <p>As many people are aware and may have experienced , after an extended period of time working on a task or project, your brain may start to wander. This can be attributed to fatigue setting in. </p>
    
    <li>Working for too long can strain your muscles and lead to pain.</li>
    <li>Humans are not biologically or physically wired to focus on one task for very long, and forcing it does not help.</li>
        <p>When your brain gets tired, you will lose concentration, be less able to absorb information, and be less able to solve problems</p>
</ol>

<h2>Some Git Basics Commands</h2>

When we want to create a new repository on our host machine, we will navigate to our desired location in the terminal and run the `git init` command.  This will initialize a git repository in the folder.  From here, we can create new files for our project using our preferred text editor or through the terminal using the `touch` command.  Once we have created our project files, the `git status` command will show us what files git knows exist and color coded red or green depending on their status.

In order to see a list of the remote servers that we have configured we use  `git remote`. The server which you clone from is labeled and known as `origin` . Personally, I find this nomenclature easier for remembering which is my original branch. If you are collaborating on a project, or just happen to have more than one remote, the command `git remote -v` will list out all of the remotes and the URLs that Git has associated with them to read and write.

To add a new remote Git repository we can run `git remote add <shortname> <url>`. To fetch the information from another collaborator that is not yet on our repository you can run `git fetch <remote>`.  Running the `git fetch` command, however, will only download the data to your local repository, but in order to merge it to what you are currently working on will require a manual merge. The `git pull` command will automatically fetch and merge the remote branch into your currently working brancy.

Once we have sharable project and want to push it upstream we use the command `git push <remote name> <branch name>`. For example, pushing your master to your origin branch would be  `git push origin master`. However, and this is something that i have run into many times in the past, pushing will only work if someone else has not pushed to the clone. If it is the case that you attempt to push after someone else, you will receive a rejection. You will have to fetch and merge the other persons work first.

