# grit

readable git

I would recommend making an alias and adding it to your `.bashrc`
```sh
alias grit='. ~/Documents/grit/grit'
```

![preview](/preview.png)

Commands:

* `grit` - list current branches and current modified files
* `grit pull [branch]` - pull branch (or develop of none provided)
* `grit push [branch]` - push to branch (or HEAD if none provided)
* `grit release` - pull master branch
* `grit diff` - show diff, ignoring whitespace changes at end of lines
* `grit commit [message]` - commit staged files with message (opens editor if none provided)
* `grit uncommit` - un-commit the last commit without losing work
* `grit amend` - amend the staged files to the last commit
