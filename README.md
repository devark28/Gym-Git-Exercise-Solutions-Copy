# Git Excersise (Commands used)

## Bundle 1

### Exercise 1

```shell
  git init
  cd git_bundle_exercises
  git remote add origin git@github.com:devark28/git_bundle_exercises.git
  echo 'Just Do It' > git_bundle_1_exercise_1/'Just Do It'
  git branch master
  git add .
  git commit -m 'Initial commit'
  git branch # list all branches
  git branch -M main
  git push --set-upstream origin main
  git branch dev
  git branch test
  git branch # list all branches
  git branch -d test
  ```

### Exercise 2

```shell
  # used vscode to create all the files (home.html, about.html, team.html)
  git branch dev2
  git checkout dev2
  cd git_bundle_1_exercise_2
  touch README.md
  touch home.html
  git add .
  git stash
  git stash list
  touch about.html
  git add .
  git stash
  git stash list
  touch team.html
  git add .
  git stash
  git stash list
  git stash list -p
  git stash pop 1
  git stash list -p
  git stash pop 1
  git stash list -p
  git commit -m 'Feat: home.html & about.html'
  git push --set-upstream origin dev2
  git stash list
  git stash list -p
  git stash pop
  git reset --hard
  ```

## Bundle 2

### Exercise 1

```shell
  cd git_bundle_exercises
  # used vscode to create all the files
  git checkout -b ft/bundle-2
  git status
  git commit -m 'Feat: created services.html'
  git branch # check current branch
  git push --set-upstream origin ft/bundle-2
  ```

### Exercise 2

```shell
  cd git_bundle_exercises
  git checkout main
  git pull
  git checkout -b ft/service-redesign
  # used vscode to create all the files
  git status
  git add -A
  git commit -m 'Feat: added services we offer'
  git push --set-upstream origin ft/service-redesign
  git checkout main
  # used vscode to edit services.html same lines
  git status
  git add -A
  git commit -m 'Feat: added services we offer'
  git push
  git checkout ft/service-redesign
  git diff main
  git merge main
  # used vscode to edit services.html to resolve the conflict
  git status
  git add services.html 
  git status
  git commit -m 'Fix: resolve conflict merging from main'
  git merge main
  git status
  git log
  git push
  ```
