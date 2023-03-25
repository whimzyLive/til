# Syncing changes from upstream

To fetch latest changes from upstream into your fork, you first need to add the upstream as one of the known git origins.

- Add origin named `upstream` to your fork running

```sh
git remote add upstream https://github.com/ORIGINAL_OWNER/ORIGINAL_REPOSITORY.git
```

- Next fetch all available branches and their commits from the upstream to your local

```sh
git fetch upstream
```

- Run following to merge changes from upstream branch to your working branch

```sh
git merge upstream/<branchname>
```
