mkdir new-project
cd new-project
git init
echo "init" > README.md
git add README.md
git commit -m "Init"
git branch -M main
git remote add origin https://github.com/vasyl-babynets/new-project.git
git push -u origin main
git checkout -b development
git add README.md
git commit -m "Add instruction"
git checkout main
git merge development