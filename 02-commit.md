### Git Commit

Git doesn't peer over your shoulder and track every keypress. Instead, at some point you will inform git that you have changed one or more files in the repository and you want it to record those changes. You do this using the _commit_ command.

For reasons, this is actually a two-step process with Git. First, you use the _add_ command to _stage_ change(s). Then you _commit_ the changes and Git records them.

```
git add some-file.c
git commit -m "this string is a commit comment"
```

#### Try it Together

Edit the file, TODO.md, and add the following lines at the bottom:

```
- learn Git
- have lunch
```

Now let's add and commit the change:

```
git add TODO.md
git commit -m "Updated TODO list with two new items"
```

Another very useful Git command, is `git status` which displays a ton of information about the state of your working directory.

Now for the time being, if you run this command, you'll need to squint and ignore a lot of the details &mdash; since there's a lot we haven't yet covered &mdash; but in a nutshell there are three important sections in the display, reading from the bottom of the screen to the top

- Untracked files - these are files that are completely unknown to Git because they haven't had `git add` run on them
- Changes not staged for commit - these are files that have been added in the past, but you have not re-run `git add` on them since making changes
- Changes to be committed - these are files whose changes have had `git add`, but you have not yet run `git commit`

Some or all of these sections may not appear depending on the state of the files in your working copy.

#### Your Turn

Do the following in your working copy:

1. Create a file; use `<LastName><FirstInitial>.txt` as the file name (e.g. my file will be named _BurkeM.txt_). Put a few lines of random text in the file.
2. Now add and commit this change.

#### Further Reading

- https://git-scm.com/book/en/v2/Git-Basics-Recording-Changes-to-the-Repository

