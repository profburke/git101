### Git Clone

In order to start working on an established project, it is necessary to get a (local) copy of the project. This is done with the `clone` command.

For example:

```
git clone git@github.com:profburke/git101.git
```

_Let's take a look at what that did..._

- The remote copy of the project is called a *repository* (_repo_ for short).
- We now have a local copy of this repository, often called a _working copy_.
- Our local repo has all the project's files. It also has a hidden subdirectory, _.git_, that is essentially a database with details of all the changes made to the project since it was initialized.

When you clone a working copy from a remote repository, by default, the remote is given the name _origin_ and you can refer to it by that name in various operations.

_One more thing..._

Git supports two different protocols. We saw SSH above. We can also use HTTP. SSH is often more convenient, but requires you to configure the remote with your SSH public key. 

#### Try it Together

Let's try cloning using HTTPS:

```
git clone https://github.com/profburke/git101.git
```


#### Your Turn

1. Clone the following repository: https://github.com/profburke/git101-sample

We will use this repository for the remaining exercises. So let me or a TA know if you encounter problems cloning this repository.

#### Further Reading

- https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository

- https://git-scm.com/book/en/v2/Git-Basics-Getting-a-Git-Repository#_git_cloning

