# git_training

---

An interactive git training meant to teach you how git works, not just which commands to execute.

Based on the general concept from Rachel M. Carmena's blog post on [How to teach Git](https://rachelcarmena.github.io/2018/12/12/how-to-teach-git.html) 

## This is currently a work in progres!

---

So, you want to use git right? 

But you don't just want to learn commands, you want to understand what you're using? 

Then this is meant for you!

Let's get started!

## Overview

In the picture below you see four boxes. One of them stands alone, while the other three are grouped together in what I'll call your _Development Environment_. 

![git components](img/components.png)

We'll start with the one that's on it's own though. The _Remote Repository_ is where you send your changes when you want to share them with other people, and where you get their changes from. If you've used other version control systems there's nothing interesting about that. 

The _Development Environment_ is what you have on your local machine. 
The three parts of it are your _Working Directory_, the _Staging Area_ and the _Local Repository_. We'll learn more about those as we start using git. 

Choose a place in which you want to put your _Development Environment_. 
Just go to your home folder, or where ever you like to put your projects. You don't need to create a new folder for your _Dev Environment_ though. 

## Getting a _Remote Repository_ 

Now we want to grab a _Remote Repository_ and put what's in it onto your machine. 

I'd suggest we use this one ([https://github.com/UnseenWizzard/git_training.git](https://github.com/UnseenWizzard/git_training.git) if for some reason you're not already reading this on github).

> To to that I can use `git clone https://github.com/UnseenWizzard/git_training.git`
> 
> But as following this tutorial will need you get the changes you make in your _Dev Environment_ back to the _Remote Repository_, and github doesn't just allow anyone to do that to anyone's repo, you'll best create a _fork_ of it right now. There's a button to do that on the top right of this page. 

Now that you have a copy of my _Remote Repository_ of your own, it's time to get that onto your machine. 

For that we use `git clone https://github.com/{YOUR USERNAME}/git_training.git`

As you can see in the diagram below, this copies the _Remote Repository_ into two places, your _Working Directory_ and the _Local Repositry_. 
Now you see how git is _distributed_ version control. The _Local Repository_ is a copy of the _Remote_ one, and acts just like it. The only difference is that you don't share it with anyone. 

What `git clone` also does, is create a new folder whereever you called it. There should be a `git_training` folder now. Open it. 

![Cloning the remote repo](img/clone.png)

## Adding new things

Someone already put a file into the _Remote Repository_. It's `Alice.txt`, and kind off lonely there. Let's create a new file and call it `Bob.txt`. 

What you've just done is add the file to your _Working Directory_. 
There's two kinds of files in your _Working Directory_: _tracked_ files that git knows about and _untracked_ files that git doesn't know about (yet). 

To see what's going on in your _Working Directory_ run `git status`, which will tell you what branch you're on, whether your _Local Repository_ is different from the _Remote_ and the state of _tracked_ and _untracked_ files. 

You'll see that `Bob.txt` is untracked, and `git status` even tells you how to change that. 
In the picture below you can see what happens when you follow the advice and execute `git add Bob.txt`: You've added the file to the _Staging Area_, in which you collect all the changes you wish to put into _Repository_

![Adding changes to the staging area](img/add.png)

When you have added all your changes (which right now is only adding Bob), you're ready to _commit_ what you just did to the _Local Repository_. 

The collected changes that you _commit_ are some meaningful chunk of work, so when you now run `git commit` a text editor will open and allow you to write a message telling everything what you just did. When you save and close the message file, your _commit_ is added to the _Local Repository_.

![Commiting to the local repo](img/commit.png)

You can also add your _commit message_ right there in the command line if you call `git commit` like this: `git commit -m "Add Bob"`. But because you want to write [good commit messages](https://chris.beams.io/posts/git-commit/) you really should take your time and use the editor.

Now your changes are in your local repository, which is a good place for the to be as long as no one else needs them or you're not yet ready to share them. 

In order to share your commits with the _Remote Repository_ you need to `push` them. 

![Pushing to the local repo](img/push.png)

Once you run `git push` the changes will be sent to the _Remote Repository_. In the diagram below you see the state after your `push`.

![State of all components after pushing changes](img/after_push.png)

## Making changes
So far we've only added a new file. Obviously the more intersting part of version control is changing files. 

Have a look at `Alice.txt`. 

It actually contains some text, but `Bob.txt` doesn't, so lets change that and put `Hi!! I'm Bob. I'm new here.` in there. 

If you run `git status` now, you'll see that `Bob.txt` is _modified_. 
In that state the changes are only in your _Working Directory_.

If you want to see what has changed in your _Working Directory_ you can run `git diff`, and right now see this: 

```Diff
diff --git a/Bob.txt b/Bob.txt
index e69de29..3ed0e1b 100644
--- a/Bob.txt
+++ b/Bob.txt
@@ -0,0 +1 @@
+Hi!! I'm Bob. I'm new here.
```

Go ahead and `git add Bob.txt` like you've done before. As we know, this moves your changes to the _Staging Area_. 

I want to see the changes we just _staged_, so let's show the `git diff` again! You'll notice that this time the output is empty. This happens because `git diff` operates on the changes in your _Working Directory_ only. 

To show what changes are _staged_ already, we can use `git diff --staged` and we'll see the same diff output as before. 

I just noticed that we put two exclamation marks after the 'Hi'. I don't like that, so lets change `Bob.txt` again, so that it's just 'Hi!' 

If we now run `git status` we'll see that there's two changes, the one we already _staged_ where we added text, and the one we just made, which is still only in the working directory. 

We can have a look at the `git diff` between the _Working Directory_ and what we've already moved to the _Staging Area_, to show what has changed since we last felt ready to _stage_ our changes for a _commit_. 

```Diff
diff --git a/Bob.txt b/Bob.txt
index 8eb57c4..3ed0e1b 100644
--- a/Bob.txt
+++ b/Bob.txt
@@ -1 +1 @@
-Hi!! I'm Bob. I'm new here.
+Hi! I'm Bob. I'm new here.
```

As the change is what we wanted, let's `git add Bob.txt` to stage the current state of the file. 

Now we're ready to `commit` what we just did. I went with `git commit -m "Add text to Bob"` because I felt for such a small change writing one line would be enough. 

As we know, the changes are now in the _Local Repository_. 
We might still want to know what change we just _commited_ and what was there before. 

We can do that by comparing commits. 
Every commit in git has a unique hash by which it is referenced. 

If we have a look at the `git log` we'll not only see a list of all the commits with their _hash_ as well as _Author_ and _Date_, we also see the state of our _Local_ and the _Remote Repsitory_. 

Right now the `git log` looks something like this: 

```ShellSession
commit 87a4ad48d55e5280aa608cd79e8bce5e13f318dc (HEAD -> master)
Author: {YOU} <{YOUR EMAIL}>
Date:   Sun Jan 27 14:02:48 2019 +0100

    Add text to Bob

commit 8af2ff2a8f7c51e2e52402ecb7332aec39ed540e (origin/master, origin/HEAD)
Author: {YOU} <{YOUR EMAIL}>
Date:   Sun Jan 27 13:35:41 2019 +0100

    Add Bob

commit 71a6a9b299b21e68f9b0c61247379432a0b6007c 
Author: UnseenWizzard <nicola.riedmann@live.de>
Date:   Fri Jan 25 20:06:57 2019 +0100

    Add Alice

commit ddb869a0c154f6798f0caae567074aecdfa58c46
Author: Nico Riedmann <UnseenWizzard@users.noreply.github.com>
Date:   Fri Jan 25 19:25:23 2019 +0100

    Add Tutorial Text

      Changes to the tutorial are all squashed into this commit on master, to keep the log free of clutter that distracts from the tutorial

      See the tutorial_wip branch for the actual commit history
```

In there we see a few interesting things: 
* The first two commits are made by me.
* Your initial commit to add Bob is the current _HEAD_ of the _master_ branch on the _Remote Repository_. We'll look at this again when we talk about branches and getting remote changes.
* The latest commit in the _Local Repository_ is the one we just made, and now we know its hash.

> Note that the actual commit hashes will be different for you. If you want to know how exactly git arrives at those revision IDs have a look at [this interesting article ](https://blog.thoughtram.io/git/2014/11/18/the-anatomy-of-a-git-commit.html)

To compare that commit and the one one before we can do `git diff <commit>^!`, where the `^!` tells git to compare to the commit one before. So in this case I run `git diff 87a4ad48d55e5280aa608cd79e8bce5e13f318dc^!`

We can also do `git diff 8af2ff2a8f7c51e2e52402ecb7332aec39ed540e 87a4ad48d55e5280aa608cd79e8bce5e13f318dc` for the same result and compare any two commits. Note that the format here is `git diff <from commit> <to commit>`, so our new commit comes second.

In the diagram below you again see the different stages of a change, and the diff commands that apply to where a file currently is. 

![States of a change an related diff commands](img/diffs.png)

Now that we're sure we made the change we wanted, go ahead and `git push`. 

## Branching

What you've just done works, because you own the _Remote Repository_. If you're working with git in most professional or open source settings, you'll notice that when you run `git push` as you've just done, you'll get an error message. 

Another thing that makes git great, is the fact that working with branches is really easy and integral part of how you work with git.

What you've done by `cloning` the _Remote Repository_ was to also automatically `checkout` it's main or _master_ branch. 

The error message you'd usually see when trying to just just `push` changes on the _master_ branch, is because branches can be _protected_, which means that not everyone is allowed to just `push` changes there. 

With this you can make sure, that changes that actually go into the main _master_ branch are reasonable. Usually you'll be working on your own _branch_, until you're done and confident in your changes which can then be `merged` into the _master. 

Don't worry, we'll get back to all of these things in more detail when we need them.  

Right now we want to create a branch to make some changes there. Maybe you just want to try something on your own and don't mess with the working state on you _master_ branch, or you're not allowed to `push` to _master_.

<!-- LIST BRANCHES -->

<!-- CHECKOUT A BRANCH -->

<!-- CREATE A NEW BRANCH -->

## Merging

<!-- MERGE TWO BRANCHES -->

<!-- NO CONFLICT -->

<!-- RESOLVE A CONFLICT -->

## Rebasing

<!-- rebase TWO BRANCHES -->

<!-- NO CONFLICT -->

<!-- RESOLVE A CONFLICT -->

## Updating the _Dev Environment_ with remote changes

<!-- fetch -->

<!-- pull -->

<!-- pull -r -->

## Cherry-picking

<!-- cherry pick from a branch -->

## Rewriting history

<!-- ammending -->

<!-- squashing -->

<!-- force pushing -->