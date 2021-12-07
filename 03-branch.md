### Git Branch

The Git commit command solves one of the problems for which we use version control: it lets us go back in time and examine the state of the project at any point in the past. It also allows us to undo changes when necessary.

There is another important ability that Git enables: allowing more than one person to easily work on the same project. The feature that enables this is _branching_.

What is a branch? A branch is similar to a cloned repository &mdash; branching gives you a new copy of your project. Once you have branched, the changes you make do not effect your original working copy unless at some point you _merge_ them. If you delete a branch without merging its changes, then it is as if you never did any of the work.

Branches are _not_ cloned repositories &mdash; for one thing, there is a lot less overhead than a clone. But thinking of branches this way is a good metaphor to start with.

```
git checkout -b experiment-1
```

I'll add a file to this branch:

```
cat > a-new-file.txt
here are my file's contents
^d

git add a-new-file.txt
git commit -m "add file to branch"
```

It turns out you've been working on a branch all along, _the main branch_. Let's switch back to it:

```
git checkout main
```

And if we list the files in our working copy, we see that `a-new-file.txt` is not there. This shouldn't be surprising: we didn't add it to the `main` branch.

#### Try it Together

Let's create a third branch: `experiment-2`:

```
git checkout -b experiment-2
```

Will we see `a-new-file.txt` on this newly-created branch? List the directory and see!

Let's switch back to the main branch:

```
git checkout main
```

#### Your Turn

1. Create a new branch called `hotfix`
2. Add a file `patch.c` (_just put 1-2 lines of random text in it_) and commit it.
3. Switch back to the main branch. Will the `` file be there?
4. Switch to the `experiment-1` branch. Which files will be there?

#### Further Reading

- https://www.atlassian.com/git/tutorials/using-branches

