# git_training

---

An interactive git training meant to teach you how git works, not just which commands to execute
Based on the general concept from Rachel M. Carmena's blog post on [How to teach Git](https://rachelcarmena.github.io/2018/12/12/how-to-teach-git.html) 

## This is currently a work in progres!

---

So, you want to use git right? 
But you don't just want to learn commands, you want to understand what you're using? 
Then this is meant for you!

Let's get started!

## Overview

In the picture below you see four boxes. One of them stands alone, while the other three are grouped together in what I'll call your `Development Environment`. 

We'll start with the one that's on it's own though. The `Remote Repository` is where you send your changes when you want to share them with other people, and where you get their changes from. If you've used other version control systems there's nothing interesting about that. 

The `Development Environment` is what you have on your local machine. 
The three parts of it are your `Working Directory`, the `Staging Area` and the `Local Repository`. We'll learn more about those as we start using git. 

Choose a place in which you want to put your `Development Environment`. 
Just go to your home folder, or where ever you like to put your projects. You don't need to create a new folder for your `Dev Environment` though. 

## Getting a _Remote Repository_ 

Now we want to grab a `Remote Repository` and put what's in it onto your machine. I'd suggest we use this one [https://github.com/UnseenWizzard/git_training.git if you're not already reading this on github](https://github.com/UnseenWizzard/git_training.git) 

For that we use `git clone https://github.com/UnseenWizzard/git_training.git` 

As you can see in the diagram below, this copies the `Remote Repository` into two places, your `Working Directory` and the `Local Repositry`. 
Now you see how git is _distributed_ version control. The `Local Repository` is a copy of the `Remote` one, and acts just like it. The only difference is that you don't share it with anyone. 

What `git clone` also does, is create a new folder whereever you called it. There should be a `git_training` folder now. Open it. 

## Adding things

Someone already put a file into the _Remote Repository_. It's `Alice.txt`, and kind off lonely there. Let's create a new file and call it `Bob.txt`. 

What you've just done is add the file to your _Working Directory_. 
There's two kinds of files in your _Working Directory_: _tracked_ files that git knows about and _untracked_ files that git doesn't know about (yet). 

To see what's going on in your _Working Directory_ run `git status`, which will tell you what branch you're on, whether your _Local Repository_ is different from the _Remote_ and the state of _tracked_ and _untracked_ files. 

You'll see that `Bob.txt` is untracked, and `git status` even tells you how to change that. 
In the picture below you can see what happens when you follow the advice and execute `git add Bob.txt`: You've added the file to the _Staging Area_, in which you collect all the changes you wish to put into `Repository`

When you have added all your changes (which right now is only adding Bob), you're ready to _commit_ what you just did to the _Local Repository_. 

The collected changes that you _commit_ are some meaningful chunk of work, so when you now run `git commit` a text editor will open and allow you to write a message telling everything what you just did. When you save and close the message file, your _commit_ is added to the _Local Repository_.

You can also add your _commit message_ right there in the command line if you call `git commit` like this: `git commit -m "Add Bob"`. But because you want to write [good commit messages](https://chris.beams.io/posts/git-commit/) you really should take your time and use the editor.

Now your changes are in your local repository, which is a good place for the to be as long as no one else needs them or you're not yet ready to share them. 

In order to share your commits with the `Remote Repository` you need to `push` them. 
However if you run `git push` you'll notice I've been mean, and _protected_ my Repositories _master_ branch, so that not everyone is allowed to just `push` changes there. You'll have to try something else if you want to share your changes. 

## Branching, Merging and Rebasing
[coming soon... if this is even any good and usefull so far]
