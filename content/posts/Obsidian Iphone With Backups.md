+++
author = "BongweKE"
title = "Free Obsidian Notes on Iphone"
date = "2025-02-12"
description = "Lorem Ipsum Dolor Si Amet"
tags = [ "obsidian", "ish", "opensource"]
weight = 10
+++

### 1. Setup GitHub in ish

Download iSH app to your iPhone and install github

```bash
$ apk add git
```

Once git is install follow the tutorial to setup  [[Github SSH]]

This will enable you to have your own backups of obsidian using open source github version control

### 2. Make an obsidian folder

Create a folder for obsidian notes on your iphone using the icloud option prefarrably

### 3. Make a new folder on ISH and mount it to the obsidian vault just created

On iSH, before opening obsidian, create  a folder either by pulling from git: 

```bash
git clone git@github.com:BongweKE/NOTES.git

mount mount -t ios . NOTES

cd NOTES/
   #follow the correct steps to get content
   #in here. pull, change branch, etc

```


In case you wanna setup a new vault, there’s a way I figured out.
Using the tutorial on [this reddit post](https://www.reddit.com/r/ish/comments/wipf6e/access_files_outside_of_ish/) I learnt these commands do the trick:

```bash
mkdir NOTES
      #follow steps on git init
mount -t ios . NOTES

```

A menu will pop up where you can choose the exact folder where your vault is located
Now it's supposed to work.

###  Things to watch out for 

- when using git add, be specific about the files you want to add. Using wildcards like `.` will take long.
- 
