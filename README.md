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

Or create a new branch (`new-feature`) based on the origin's `main`:
```sh
grit bronch main new-feature
```

### Commands

| Command | Description |
|----------------------------------|--------------------------------------------------------------------------|
| `grit` | list current branches and current modified files |
| `grit help COMMAND` | show function body (or general help text if blank) |
| `grit pull [BRANCH]` | pull branch (develop if blank) |
| `grit push [BRANCH]` | push to branch (HEAD if blank) |
| `grit force [BRANCH]` | push to branch (HEAD) if asked nicely |
| `grit update` | pull main branch |
| `grit refresh [SOURCE] [TARGET]` | pull source branch (develop if blank) and push to target (HEAD if blank) |
| `grit bronch [SOURCE] TARGET` | create a new branch from source (develop if blank) |
| `grit dif` | show diff of words, ignoring whitespace changes |
| `grit diff` | show diff, ignoring whitespace changes |
| `grit init [ORIGIN]` | initialize a new repo (with origin if provided) |
| `grit safe` | run 'git config --global --add safe.directory $PWD' |
| `grit commit [MESSAGE]` | commit staged files with message (opens editor if blank) |
| `grit cad PATH [MESSAGE]` | add path and commit with message (opens editor if blank) |
| `grit lad` | add last diff'd file |
| `grit cal [MESSAGE]` | add last diff'd file commit with message (opens editor if blank) |
| `grit uncommit` | un-commit the last commit without losing work |
| `grit amend` | amend the staged files to the last commit |
| `grit sad NAME ORIGIN [BRANCH] [PREFIX]` | add subtree to repo with name, use branch (HEAD if blank) and use subfolder (NAME if blank) |
| `grit sup NAME [BRANCH] [PREFIX]` | update subtree by name, branch (HEAD if blank), and subfolder (NAME if blank) |
| `grit suc [command]` | for each submodule run a command |
| `grit url [URL]` | get the current remote origin url (or set it if provided) |
