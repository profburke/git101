### Git Merge

We've now seen how to get changes from the remote repository into your (local) working directory. But suppose you are working on a branch named `cool-new-feature` and a colleague of yours has incorporated some highly useful new utility functions into `origin`. 

If you `pull`, those changes will show up in your local main branch, not the branch you are working on. How do you get changes from one branch to the other?

Well, I'm sure you've guessed from the title of this section: you use the Git `merge` command.

```
git merge main
```

The `merge` command takes a parameter &mdash; the name of the branch that you want to merge into the branch on which you are currently working.

#### Try it Together

First, let's make sure we're on the main branch:

```
git checkout main
```

Now, let's add the item `- Become proficient at merging` to `Todo.md`, and commit the change:

```
git add TODO.md
git commit -m "added merge item to TODO list"
```

We switch to our `experiment-1` branch:

```
git checkout experiment-1
```

Look at TODO.md and make sure our new item is *NOT* there.

Now, let's merge our change from the main branch:

```
git merge main
```

#### Your Turn

While still in the branch `experiment-1`, do the following:

1. Add `- Prepare for hackathon` to `TODO.md`.
2. Commit the change
3. Merge the change back into your main branch


#### Further Reading
