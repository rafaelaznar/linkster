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

* How to merge two repos presenving history: https://stackoverflow.com/questions/1425892/how-do-you-merge-two-git-repositories
* About GITHUB renaming master branch to main: 
  * 'master' word is considered offensive by some, and so it was replaced with ‘main’, but in the context of git, the word “master” is not used in the same way as “master/slave”. Master in git is derived from the Latin word “magester”, meaning chief or teacher. The consequence is that if you don't want to end up with two branches, main and master, you to rename master to main in every new project before push to github in order to eliminate master.
  * https://medium.datadriveninvestor.com/why-githubs-change-from-master-to-main-is-not-the-solution-a3ac38cc48dd
  * https://github.com/github/renaming
* Revert github commits: 
  - Clone proyect
  - Localy perform a hard reset to the last commit you want to preserve
  - From command line execute a forced push: 
```git git push origin master --force ```
  * from: https://stackoverflow.com/questions/448919/how-can-i-remove-a-commit-on-github
* Setting origin & upstream
```git
git remote add origin https://github.com/rafaelaznar/angular-router-example-02.git
git remote -v
git set-url origin https://github.com/rafaelaznar/angular-router-example-02.git
```
* setting autor and email: IMPORTANT: note that if you don't set the author's email, Github won't consider your contributions as yours!
```git
git config –global user.name "Your Name"
git config –global user.email "you@example.com"
```
  * you can also fix your identity: ```git git commit –amend –reset-author ```
