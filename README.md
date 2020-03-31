git rev-list --count HEAD
git rev-list --count HEAD ^<branch-name>
  
If you don't want to count these commits add --no-merges:

git rev-list --no-merges --count HEAD ^develop


---To see total no of commits
git rev-list --count HEAD


---To see total no of commits by person
git shortlog -s -n
---This gives me an exact count of commits in the current branch having its base on master
git rev-list --count develop..HEAD

---How much commits was done to current branch since begin of history, not counting commits from merged branches:
git rev-list HEAD --count --first-parent

---number of commits done since some other commit:
git rev-list HEAD abc0923f --count --first-parent

---Count commits done since 2018 year
git rev-list HEAD --count --first-parent --since=2018-01-01
