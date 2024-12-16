# Used commands

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
