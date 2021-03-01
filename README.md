# Git setup

Git - basic setup

## Basic Configuration

I prefer global configuration (using `--global`) stored in your home directory applied to all repositories.

You can configure just one repo, you can call `git config` from you repository with flag `--local`.

```
git config --global user.name "Name Surname"
git config --global user.email "name@surname.com"
```

### Setup default git Editor

Git use by default Vim or editor from `EDITOR` environment variable. If you want to use different editor, you can configure it.

```
git config --global core.editor nano
```

### Rebase workflow (if you want to use rebase workflow)

**WARNING**: Apply only if you want to use rebase workflow!

```
git config --global pull.ff only
git config --global merge.ff only
git config --global pull.rebase true
```
