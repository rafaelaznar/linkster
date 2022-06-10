# Git Selected Online Links
* https://en.wikipedia.org/wiki/Git

## CheatSheets

* https://education.github.com/git-cheat-sheet-education.pdf

## Tutorials & reference books

* https://www.atlassian.com/git/tutorials
* https://rogerdudler.github.io/git-guide/
* https://docs.github.com/es
* https://git-scm.com/book/en/v2

## Interesting links

### Merge two repos
How to merge two repos presenving history: https://stackoverflow.com/questions/1425892/how-do-you-merge-two-git-repositories

### Revert github commits: 
  - Clone project
  - Localy perform a hard reset to the last commit you want to preserve
  - From command line execute a forced push: ```git push origin master --force ```
  * from: https://stackoverflow.com/questions/448919/how-can-i-remove-a-commit-on-github

### Setting origin & upstream
```git
git remote add origin https://github.com/rafaelaznar/angular-router-example-02.git
git remote -v
git set-url origin https://github.com/rafaelaznar/angular-router-example-02.git
```
### Setting identity 
IMPORTANT: note that if you don't set the author's email, Github won't consider your contributions as yours!
```git
git config –global user.name "Your Name"
git config –global user.email "you@example.com"
```
* you can also edit manually ~/.gitconfig
```
[user]
email = myemail@mydomain.net
name = Rafael Aznar
```
* you can fix identity for a commit: ```git commit –amend –reset-author ```
  * ```git commit --amend --author="Author Name <email@address.com>" --no-edit```
  * https://stackoverflow.com/questions/3042437/how-to-change-the-commit-author-for-one-specific-commit

### Creating a repo:
```
Create repo in github mysourcerepo (note master now is main branch)
Localy:
  git init
  git add .
  git commit -m "first commit"
  git branch -M main
  git remote add origin https://github.com/rafaelaznar/mysourcerepo
  git pull origin main –allow-unrelated-histories
  git push -u origin main (need your token)
```

### Number of Code lines (SLOC) in a git project:
```bash
#!/usr/bin/env bash
git clone --depth 1 "$1" temp-linecount-repo &&
  printf "('temp-linecount-repo' will be deleted automatically)\n\n\n" &&
  cloc temp-linecount-repo &&
  rm -rf temp-linecount-repo
```
* call example: ```raznara@SP-PC01:~$ ./cloc-git https://github.com/rafaelaznar/my-project.git```
* https://stackoverflow.com/questions/26881441/can-you-get-the-number-of-lines-of-code-from-a-github-repository
* also see command ```git ls-files | xargs wc -l``` from https://gist.github.com/mandiwise/dc53cb9da00856d7cdbb

### Git and prompt
* Activate colors
```
git config --global color.status auto
git config --global color.branch auto
```
you can also edit manually ~/.gitconfig
```
[color "status"]
  added = blue 
  changed = yellow 
  untracked = white ul
[color "diff"]
  meta = white bold
  frag = magenta ul 
  old = red bold
  new = green bold
[color]
  ui = auto
  branch = auto
```
* Showing branch: you should add this lines to the .bashrc lines
```
function parse_git_dirty {
  status=`git status 2> /dev/null`
  dirty=`    echo -n "${status}" 2> /dev/null | grep -q "Changed but not updated" 2> /dev/null; echo "$?"`
  untracked=`echo -n "${status}" 2> /dev/null | grep -q "Untracked files" 2> /dev/null; echo "$?"`
  ahead=`    echo -n "${status}" 2> /dev/null | grep -q "Your branch is ahead of" 2> /dev/null; echo "$?"`
  newfile=`  echo -n "${status}" 2> /dev/null | grep -q "new file:" 2> /dev/null; echo "$?"`
  renamed=`  echo -n "${status}" 2> /dev/null | grep -q "renamed:" 2> /dev/null; echo "$?"`
  bits=''
  if [ "${dirty}" == "0" ]; then
    bits="${bits}☭"
  fi
  if [ "${untracked}" == "0" ]; then
    bits="${bits}?"
  fi
  if [ "${newfile}" == "0" ]; then
    bits="${bits}*"
  fi
  if [ "${ahead}" == "0" ]; then
    bits="${bits}+"
  fi
  if [ "${renamed}" == "0" ]; then
    bits="${bits}>"
  fi
  echo "${bits}"
}
 
function parse_git_branch {
  git branch --no-color 2> /dev/null | sed -e '/^[^*]/d' -e "s/* \(.*\)/(\1$(parse_git_dirty))/"
}
 
export PS1='\[\033[00;32m\]\u\[\033[01m\]@\[\033[00;36m\]\h\[\033[01m\] \! \[\033[00;35m\]\w\[\033[00m\]\[\033[01;30m\]$(parse_git_branch)\[\033[00m\]\$ '
```
* more sources for the prompt:
  * https://gist.github.com/monde/217120
  * https://github.com/twolfson/sexy-bash-prompt
  * http://lancespeelmon.wordpress.com/2012/05/10/three-tips-for-creating-the-best-ever-git-command-line/
  * http://oliverdavies.co.uk/blog/2013/04/display-git-branch-or-tag-names-your-bash-prompt
* autocomplete git commands from terminal: 
  * download .git-completion.bash and place it at home
  * add this code to .bashrc:
```
if [ -f ~/.git-completion.bash ]; then
    . ~/.git-completion.bash
fi
```



### About GITHUB renaming master branch to main
  * 'master' word is considered offensive by some, and so it was replaced with ‘main’, but in the context of git, the word “master” is not used in the same way as “master/slave”. Master in git is derived from the Latin word “magester”, meaning chief or teacher. The consequence is that if you don't want to end up with two branches, main and master, you to rename master to main in every new project before push to github in order to eliminate master.
  * https://medium.datadriveninvestor.com/why-githubs-change-from-master-to-main-is-not-the-solution-a3ac38cc48dd
  * https://github.com/github/renaming
