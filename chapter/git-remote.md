## Common `git remote` Command

Git Remote manages the set of remotes that you are tracking with your local repository.

```
# List the current remotes associated with the local repository
git remote -v

# Add a remote
git remote add [name] [URL]

# Remove a remote
git remote remove [name]
```

## What is `origin`?

If you try running `git remote -v` in your repositories, you'll probably see something called `origin`. You may notice `origin` in many messages from Git. `origin` is the human-friendly name for the URL that the remote repository is stored at. It's like a key value pair, and `origin` is the default.

## What is `upstream`?

You may need or want to work with multiple remotes for one local repository. This can be common in open source, when a contributor needs to create a fork of a repository to have permission to push changes to the remote.

In this case, it's common to create and clone a fork. Then, the default remote would be `origin`, in reference to the fork. To make it easier to pull any changes to update the local copy of the fork from the original repository, many people add the original repository as a remote also. It's typical to name this remote `upstream`.

**NOTE:** [READ MORE](https://github.com/git-guides/git-remote)