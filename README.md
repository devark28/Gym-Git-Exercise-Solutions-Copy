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
