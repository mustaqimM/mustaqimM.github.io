  Command line instructions
Git global setup

git config --global user.name "Mustaqim"
git config --global user.email "mustaqim@protonmail.com"

Create a new repository

git clone https://gitlab.com/mustaqim/pass.git
cd pass
touch README.md
git add README.md
git commit -m "add README"
git push -u origin master

Existing folder

cd existing_folder
git init
git remote add origin https://gitlab.com/mustaqim/pass.git
git add .
git commit
git push -u origin master

Existing Git repository

cd existing_repo
git remote add origin https://gitlab.com/mustaqim/pass.git
git push -u origin --all
git push -u origin --tags
