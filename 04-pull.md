### Git Pull

Suppose your colleague makes changes to the project and incorporates those changes in the remote repository (_How? We haven't learned that yet. Assume magic for the time being._)

Further suppose you want to get those changes from the remote repository and incorporate them in your working copy.

`Pull` to the rescue.

![git pull image](images/pull.png)

The basic form of the command is quite simple

```
git pull
```

Recall earlier I said that one reason to use Git was that it allowed two or more people to make changes without trampling on each others' work.

What if you and I both edit the same file and I pull in your changes? Usually that's not a problem. The file will now have your changes and my work will be unaffected.

Usually isn't always. What happens if there's a problem? For the answer to that question, you'll have to wait for section 7.

#### Your Turn

While you weren't looking, I've updated the `git101-sample` remote with some changes.

1. Pull those changes into your working copy.

If you now look at the contents of the TODO file, you should now see the _learn Git_ and _lunch_ items I added earlier to my local repo!

#### Further Reading

- https://www.atlassian.com/git/tutorials/syncing/git-pull

- https://www.atlassian.com/git/tutorials/syncing/git-fetch

