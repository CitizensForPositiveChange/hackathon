### Hackathon notes

#### Git 101 :)

- Start by cloning this repository onto your local machine

git clone git@github.com:CitizensForPositiveChange/hackathon.git

- It is good practice to always pull from master before creating a new branch. This will help you avoid merge conficts in the future!

git pull origin master

- Let's create a new branch for updating the README

git checkout -b update_readme

- Now that we are in the update_readme branch, add whatever changes you like to the file

- Once you are ready, now we need to let git know that you have changes you would like to commit

git add README.md
git commit -am 'add some message here describing the changes you made'

- Now we are going to push this branch up to github to share.  In this case you want to push the changes you made on the update_readme branch to github (github = origin)

git push origin update_readme

