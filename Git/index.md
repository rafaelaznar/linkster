# Git Selected Links
* https://en.wikipedia.org/wiki/Git

## CheatSheets

* https://education.github.com/git-cheat-sheet-education.pdf

## Tutorials

* https://www.atlassian.com/git/tutorials
* https://rogerdudler.github.io/git-guide/

## Interesting links

* How to merge two repos presenving history: https://stackoverflow.com/questions/1425892/how-do-you-merge-two-git-repositories
* About GITHUB renaming master branch to main: 
  * 'master' word is considered offensive by some, and so it was replaced with ‘main’, but in the context of git, the word “master” is not used in the same way as “master/slave”. Master in git is derived from the Latin word “magester”, meaning chief or teacher. The consequence is that if you don't want to end up with two branches, main and master, you to rename master to main in every new project before push to github in order to eliminate master.
  * https://medium.datadriveninvestor.com/why-githubs-change-from-master-to-main-is-not-the-solution-a3ac38cc48dd
  * https://github.com/github/renaming
* Revert github commits: 
  - Clone proyect
  - Localy perform a hard reset to the last commit you want to preserve
  - From command line execute a forced push: git push origin master --force
  * from: https://stackoverflow.com/questions/448919/how-can-i-remove-a-commit-on-github
