### Git Commit

Git doesn't peer over your shoulder and track every keypress. Instead, at some point you will inform git that you have changed one or more files in the repository and you want it to record those changes. You do this using the `commit` command.

This is actually a two-step process with Git, _for reasons_. First, you use the `add` command to _stage_ change(s). Then you _commit_ the changes and Git records them.

```
git add some-file.c
git commit -m "this string is a commit comment"
```

![git commit image](images/commit.png)

With the above two commands,  I have added and committed a new file to my repo. I follow the same process when I make changes to an existing file.

First, I'll edit the file, TODO.md, and add the following lines at the bottom:

```
- learn Git
- have lunch
```

Now I'll add and commit the change:

```
git add TODO.md
git commit -m "Updated TODO list with two new items"
```

Another very useful Git command, is `git status` which displays a ton of information about the state of your local repo.

For the time being, if you run `git status`, you'll need to squint and ignore a lot of the details &mdash; there's a lot we haven't yet covered &mdash; but in a nutshell, there are three important sections in the display, reading from the bottom of the screen to the top

- **Untracked files**: these are files that are completely unknown to Git because they haven't been added (`git add <newfile>`)
- **Changes that are not staged**: these are files that have been added in the past, but since their last commit, they have been changed, and these changes were not added
- **Changes to be committed** - these are files whose changes have been staged, but you have not yet run `git commit`

Some or all of these sections may not appear depending on the state of the files in your working copy.

#### Your Turn

Do the following in your working copy of the git101-sample project:

(_I recommend you run `git status` before each step so you can get comfortable reading its output._)

1. Create a file; use `<LastName><FirstInitial>.txt` as the file name (_e.g. my file will be named `BurkeM.txt`_). Put a few lines of random text in the file.
2. Add and commit this change.
3. Make some edits you your file.
4. Add and commit this new change.

#### Further Reading

- https://git-scm.com/book/en/v2/Git-Basics-Recording-Changes-to-the-Repository

