# Git Workshop


## Get Started with git.

### git init

This creates a hidden folder, `.git` , which contains the plumbing needed for Git to work.
Next, check what ﬁles Git will add to your new repository; this step is worth special care.

```bash
git init

```

### git status

Review the resulting list of ﬁles; you can tell Git which of the ﬁles to place into version control (avoid adding ﬁles
with conﬁdential information such as passwords, or ﬁles that just clutter the repo

```bash
git status
```

### git add
```bash
git add <file/directory name #1> <file/directory name #2> < ... >
```
If all ﬁles in the list should be shared with everyone who has access to the repository, a single command will add
everything in your current directory and its subdirectories.

```bash
git add .
```

This will "stage" all ﬁles to be added to version control, preparing them to be committed in your ﬁrst commit.
For ﬁles that you want never under version control, create and populate a ﬁle named .gitignore before running
the add command.

### git commit

Commit all the ﬁles that have been added, along with a commit message

```bash
git commit -m "Initial commit"
```
This creates a new commit with the given message. A commit is like a save or snapshot of your entire project. You
can now push, or upload, it to a remote repository, and later you can jump back to it if necessary.
If you omit the -m parameter, your default editor will open and you can edit and save the commit message there.

### git remote

To add a new remote, use the `git remote` add command on the terminal, in the directory your repository is stored
at.
The `git remote` add command takes two arguments:

1. A remote name, for example, origin
2. A remote URL, for example, `https://<your-git-service-address>/user/repo.git`

```bash
git remote add origin https://<your-git-service-address>/owner/repository.git
```
>Before adding the remote you have to create the required repository in your git service, You'll be able to
push/pull commits after adding your remote.

### git push
it's time to push your codes to repo.

```bash
git push -u origin master
```

