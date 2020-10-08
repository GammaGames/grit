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

Or create a new branch (`new-feature`) based on the origin's `master`:
```sh
grit bronch master new-feature
```

### Commands

| Command                          | Description                                                              |
|----------------------------------|--------------------------------------------------------------------------|
| `grit`                           | list current branches and current modified files                         |
| `grit help [command]`                           | show function body (or general help text if blank)                         |
| `grit pull [branch]`             | pull branch (develop if blank)                                           |
| `grit push [branch]`             | push to branch (HEAD if blank)                                           |
| `grit force [branch]`            | push to branch (HEAD) if asked nicely                                    |
| `grit update`                    | pull master branch                                                       |
| `grit refresh [source] [target`] | pull source branch (develop if blank) and push to target (HEAD if blank) |
| `grit bronch [source] <branch>`  | create a new branch from origin/source (develop if blank)                |
| `grit dif`                       | show diff of words, ignoring whitespace changes                          |
| `grit diff`                      | show diff, ignoring whitespace changes                                   |
| `grit init [origin]`             | initialize a new repo (with origin if provided)                          |
| `grit commit [message]`          | commit staged files with message (opens editor if blank)                 |
| `grit cad <path> [message]`      | add path and commit with message (opens editor if blank)                 |
| `grit cal [message]`             | add last diff'd file commit with message (opens editor if blank)         |
| `grit uncommit`                  | un-commit the last commit without losing work                            |
| `grit amend`                     | amend the staged files to the last commit                                |
| `grit sup`                       | for each submodule pull the latest master branch                         |
| `grit sut`                       | for each submodule pull the latest tag                                   |
| `grit suc`                       | for each submodule run a command                                         |
