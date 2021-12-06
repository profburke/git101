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

#### Your Turn

Do the following in your working copy:

1. Create a file; use `<LastName><FirstInitial>.txt` as the file name (e.g. my file will be named _BurkeM.txt_). Put a few lines of random text in the file.
2. Now add and commit this change.

#### Further Reading

- https://git-scm.com/book/en/v2/Git-Basics-Recording-Changes-to-the-Repository

