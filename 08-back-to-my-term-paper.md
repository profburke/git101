### Term Paper Revisited

Now that we have some understanding of Git, let's look at how Git could help with our example of writing a term paper. Specifically, let's address each of the questions from that discussion.

- Which version did copy when I sent it to Takeshi? 

When you're reading for Takeshi to take a look, you can create a branch, _call it something like `takeshi-review`_. 

(_Alternatively you could use tags, but we didn't discuss those._)

- And how do I incorporate his changes?

If Takeshi uses Git, he could check out the appropriate branch, commit and push changes and you can then merge them into the main branch (_If you decide to keep his suggestions._)

We mentioned several capabilities we would like in a version control system. Let's look at those as well:

- go back to a previous state (e.g. what did this project look like last week)

We mentioned how Git keeps a record of every change to every file in the project. Consequently, Git has all the information it needs to perform this request.

- undo a change

Essentially, the same answer as above.

- track who made which change when

We discussed commits, I'll mention that each commit, in addition to recording _what_ changed, records a timestamp and the name of the person making the change.

- work with one or more colleagues (without trampling over each other's work)

Branch, push, pull, merge.

- try an experiment; maybe keep it, maybe not

Again branching.
