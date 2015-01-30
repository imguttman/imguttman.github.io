---
layout: post
title: "Git, Github, and Version Control"
date:   2014-11-23 12:30:00
categories: blog
---
This is a second-hand account extolling the virtues of version control. By that I mean that even though I have a good sense of how version control works, I haven’t utilized it in the ways that make it most useful to the programming community. To me, this lack of experience makes for a pretty significant gap in knowledge, but, suspending my doubts for the time being, here’s a quick primer on version control:

What is version control? It’s a way programmers save their work. Through version control programs like git, you can save your work in a way that’s different from how you save a document in Word. Version control enables you to save a “snapshot” of your progress – this snapshot includes a file or a group of files, and more importantly, the snapshot does not overwrite any previous snapshots.

Why is this so great? Honestly I can’t vouch for it personally since I haven’t worked on anything that requires a massive amount of code or built programs with complex interplay between different files, but from what I’ve read, version control is a way to minimize risk while working on complex project with a team of programmers. Not only does it provide the individual programmer peace-of-mind that he/she can fall back on the previous snapshot when he/she experiments with new code, it also ensures that the group members’ contributions don’t conflict when added to the master file.

How does git help you keep track of changes?
Git is popular program known for its easy-to-use version control system. Git users take snapshots through the ‘commit’ command. With every commit, user can append a description of the change that they’ve made. These descriptions are easily accessible through the ‘log’ (written ‘git log’ in the terminal) command, so users can identify and locate previous versions.

Why use GitHub to store your code?

GitHub is an important tool that makes the amplifies the usefulness of git.

Since git is a program that you download to a personal computer – just like Spotify or Skype – the different snapshots/versions created and stored by git exist only your local computer. To tap into the true power of a version control program like git, many different people must be able to retrieve code from and contribute to a remote location which, because  I lack the technical knowledge to explain how it works, I will refer to as The Cloud.  GitHub is A Cloud. It stores the master version of a project. Group members can “pull” or retrieve different files (or all the files) from a project and make modifications. They then submit their changes by “pushing” or uploading the newly modified files back up to the Cloud of GitHub. Ideally, another group member will approve this contribution and merge it with the master file. This controlled flow of information aims to prevent five group members from (unknowingly) making redundant/conflicting changes to the master file. I can’t vouch for it personally quite yet, but if the internet articles are true, then it does a good job.
