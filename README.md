# Upload TechDegree Projects Best Practice

## Table of contents

- [General](#general)
- [GitHub Pages](#gitHub-pages) 
- [Git Ignore](#git-ignore) 
- [Verification Badges](#verification-badges) 

## General
Go to your project folder and run `git init` to initialize empty git repository by default we are on the master branch 
but we need to be on the branch called "gh-pages" for project pages,
so we use the command `git checkout -b gh-pages` to create new gh-pages branch and switch to it. If we run the `git status` command we see we are on "gh-pages" branch. next we run `git add .` command to add all files and then `git commit -m "Initial commit"` to make the commit.

## GitHub Pages
In order to make it easier for someone to see your project live It highly recommend to use GitHub Pages, GitHub's free Hosting service.

**Please Note:** GitHub Pages only support front-end websites. 


To start we create a new repository and name it to the TechDegree project name here as example we set it to "TechDegree-project" and then add a short description and then click Create repository button.

**Note:** Do not check "Initialize this repository with a README" option. Also leave the "Add .gitignore" and "Add a license" options

Now copy `git remote add origin https://github.com/username/TechDegree-project.git` and paste it into the console to create remote connection to GitHub. next we type `git push orgin gh-pages` to push the code up to GitHub

## Git Ignore
Depending on the operating system and IDEs you are using there are some additional files like .DS_store files which known as junk and you really dont need them to put in your project and in the Git so here we will use .ignore file to ignore those files .It's usually used to avoid committing transient files from your working directory that aren't useful to other collaborators, such as compilation products, temporary files IDEs create, etc.
Put the .gitignore template file in your project.

## Verification Badges
To show the world which your project is valid regards to W3 and make it easier for peer reviewers to validate your code we Add this lines to your README file:

For HTML validation:
 
`[![Valid XHTML 1.0!](http://www.w3.org/Icons/valid-xhtml10)](https://validator.w3.org/check?uri=https://username.github.io/TechDegree-project/)`

For CSS validation:

`[![Valid CSS!](http://www.w3.org/Icons/valid-css.png)](https://jigsaw.w3.org/css-validator/validator?uri=https://username.github.io/TechDegree-project/)`

dont forget to change `username` with your GitHub username and `TechDegree-project` with your project name.
