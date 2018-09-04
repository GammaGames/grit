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
* `grit push [branch]` - push to branch (or HEAD if non provided)
* `git release` - pull master branch
