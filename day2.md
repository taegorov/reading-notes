### Table of Contents
[Home](README.md)

[Reading Day 1](read02.md)

[Read04](read04.md)

# Reading Notes Day 2

## Version Control

Version Control System (VCS)

Version Type | Notes
------------ | -------------
Local Version Control (Local VCS) | The content lives on your hard drive
Centralized Version Control (CVCS) | Came about due to a need for collaboration <br> Files stores on a server <br> Can be accessed by multiple users <br> **Collaborative**
Distributed Version Control (DVCS) | Like a CVS, but files (repositories) are stored in multiple places <br> **Git is a DVCS**

## What is Git?

Git saves "snapshots" of your project each time you "commit." "Commit" is sort of like "save current version," where previous versions of the file are saved as well. 

You can work on projects even when not connected to the internet, then upload later.

Git protects against file corruption and irreversible file damage.

#### [Git States](https://blog.udemy.com/wp-content/uploads/2015/08/image066.png)

State | Notes
------------ | -------------
Committed | Data is saved on your hard drive (or local database)
Modified | Data is changed but not "saved" (committed)
Staged | File ready to be committed

## Add - Commit - Push

How your workflow should look.

**Add** changes

**Commit** or save those changes

**Push** those changes to a service like GitHub


## Useful Commands

`git status` displays whether your 'branch' is up to date or not

`git add <file>` adds a repository to your local computer

`git commit -m "type your message here"` commits your changes. Make sure to add a message reflecting what specific changes were made. **THESE CHANGES ARE PUBLIC AND POTENTIAL EMPLOYERS WILL SEE THEM**

`git push origin main` syncs your changes with your GitHub page 


## Lab 03
This is where I have added more notes for Lab: 03

These notes were added via *Visual Studio Code,* then pushed to GitHub via *Ubuntu* 