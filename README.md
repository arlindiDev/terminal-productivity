## terminal-productivity


### Download gh
1. Open a terminal
2. `brew install gh`

### Setup terminal aliases
1. run `open ~/.zshrc`
2. add the following to the `.zshrc` file:
```
# build and launch app from terminal
alias runapp='./gradlew :app:deployDebug'

# short alias for ./gradlew task becomes gw task
alias gw='./gradlew'

# interacting with github
alias ghv='gh pr view --web'
alias ghc='gh pr comment --body "ci-build"'
alias ghcreate='gh pr create --fill'
alias gitap='git add . && git commit --amend --no-edit && git push -f'
alias gitmp='git checkout master && git pull' 

GITHUB_TOKEN=<GITHUB_TOKEN>

# short alias for adb location
alias adb=<YOUR_ADB_LOCATION> 

# if you are lazy to open the curtains
alias weather="curl -4 wttr.in/${1:-berlin}"
```

### Search Terminal

#### You can search your terminal for previously commands for example:
1. open a terminal
2. execute `echo "hello"`
3. execute `echo "noice"`

#### Search for the `echo "hello"`
1. hit `control+r`
2. write he
3. hit enter, the `echo "hello"` command is executed

#### Search for the `echo "hello"` but by going through all previous echo commands
1. hit `control+r`
2. write ec
3. hit `control+r` again
4. hit enter, the `echo "hello"` command is executed


