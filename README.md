# grit

readable git

I would recommend making an alias and adding it to your `.bashrc`
```sh
alias grit='. ~/Documents/grit/grit'
```

![preview](/preview.png)

Using grit you can create and push the first commit with the following:
```sh
grit init https://github.com/username/repo.git
grit cad . "Initial commit"
grit push
```

### Commands:

* `grit`                      list current branches and current modified files
* `grit pull [branch]`        pull branch (or develop of none provided)
* `grit push [branch]`        push to branch (or HEAD if none provided)
* `grit force [branch]`       force push to branch (or HEAD) if asked nicely
* `grit update`               pull master branch
* `grit diff [path]`          show diff, ignoring whitespace changes
* `grit init [origin]`        Initialize a new repo (with the given origin if provided)
* `grit commit [message]`     commit staged files with message (opens editor if none provided)
* `grit cad [path] [message]` add path and commit with message (opens editor if none provided)
* `grit uncommit`             un-commit the last commit without losing work
* `grit amend`                amend the staged files to the last commit
* `grit sup`                  for each submodule pull the latest master branch
* `grit sut`                  for each submodule pull the latest tag
* `grit suc [command]`        for each submodule run a command
