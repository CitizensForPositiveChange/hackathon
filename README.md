### Hackathon notes

#### Collaborative git 101 :)

- This website provides a very helpful intro with great diagrams, although doesn't provide info on how to do the same tasks via the command line.

https://guides.github.com/activities/hello-world/

- So here's a little git command line 101 :)

- Start by cloning this repository onto your local machine

```
git clone git@github.com:CitizensForPositiveChange/hackathon.git
```

- if the above throws an error try

```
git clone https://git@github.com/CitizensForPositiveChange/hackathon.git
```

- You just cloned a copy of the master branch on to your local machine from the 'origin' or from github.  The master branch contains the master copy of all our collaborative code.

- It is good practice to always pull from master before creating a new branch. This will help you avoid merge conflicts in the future!

```
git pull origin master
```

- If you get an error, make sure to cd into the repo directory (that has the .git directory) and then pull.

- Let's create a new branch for updating the README

```
git checkout -b update_readme
```

- Type the following to see see all local branches of your repository. The starred branch is your current branch:

```
git branch
```

- Now that we are in the update_readme branch, add whatever changes you like to the file

- Once you are ready, now we need to let git know that you have changes you would like to commit

```
git add README.md
git commit -am 'add some message here describing the changes you made'
```

- Now we are going to push our branch up to github to share.  In this case you want to push the changes you made on the update_readme branch to github (github = origin)

```
git push origin update_readme
```

- Now if we look at https://github.com/CitizensForPositiveChange/hackathon you will see 'Your recently pushed branches.'

- Click on 'Compare & pull request'

- This will open up the next page to show you the changes you made. On this page click the green button 'Create pull request'

- Now you have created a pull request, which is a request to merge your code branch into the master branch (our group code)

- From here, you will get the green thumbs up that you can merge your code or a warning that there are merge conflicts

- If you get a green thumbs up, go ahead and click the green button 'Merge pull request'

- Viola! Now your code is merged into the master code base

- Now back in your command line, we want to return back to our master branch and make sure to update the code on our local machine to match the most up-to-date code living in the master branch on github.

```
git checkout master
git pull origin master
```

- Now I personally like to delete my old branch and create a new branch off of master. It keeps life simple.

```
git branch -D update_readme
git checkout -b more_updates
```

- And keep on hacking away :)
