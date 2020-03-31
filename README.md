git rev-list --count HEAD
git rev-list --count HEAD ^<branch-name>
  
If you don't want to count these commits add --no-merges:

git rev-list --no-merges --count HEAD ^develop


---To see total no of commits
git rev-list --count HEAD


---To see total no of commits by person
git shortlog -s -n

git rev-list --count develop..HEAD
