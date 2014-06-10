git-qdiff
=========

So you miss `bzr qdiff` ?
-------------------------

Of course you do ! Why would you be there ?

Installation
------------

Just type this in your terminal:

    sudo wget https://raw.githubusercontent.com/amigrave/git-qdiff/master/git-qdiff -P /usr/local/bin
    sudo chmod +x /usr/local/bin/git-qdiff

Dependencies
------------

- git (1.7.11+)
- bazaar
- qbzr tools
- rsync

Usage
-----

Once installed, you should be able to use this command from any git repository:

    git qdiff

Of course you can use the same notations as you would with `git diff`:

```bash
# Show both staged and unstaged changes
git qdiff HEAD

# Using tilde and carrets
git qdiff HEAD~2..HEAD~3

# Between commits
git qdiff 53c43de..7c70faf

# Between branches
git qdiff my_feature..origin/master

# ...
```

Known problem
-------------

- `Refresh` button won't work

Before reporting an issue, please check that your `bzr qdiff` tool works well.
