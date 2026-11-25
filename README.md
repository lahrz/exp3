# exp3
mkdir exp3
cd exp3
git init -b master

echo "Hello Git" > exp.txt
git add exp.txt
git commit -m "initial commit"

echo "New changes" >> exp.txt
git status
git diff
cat exp.txt

git stash
git status

git checkout -b test
git checkout master

git stash pop
cat exp.txt
git status
