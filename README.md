# pratica_git_flow
Esta es la rama development

1.- The first thing we have to do is configure an SSH key. To do it, what we have to do is run the following command line in the git console :

```
$ ssh-keygen
```
The ssh key will be generated in the user's/pc default address in the .ssh directory. What we have to do is open the .pub file and copy the content 

2.- Now the next step will be to go to our github and continue to the configuration / SSH and GPG keys and add a new key where we will have to give the key a name and enter the key generated from the .pub file 

3.- The next step is to create a public repository with the name "practica_git_flow" and add a default README file 

4.- In the git console we will have to clone the github that we just created with the SSH key with the command: 
```
$ git clone git@github.com:"github_name"
```
5.- To create a branch "development" what we have to do is enter the command: 
```
$ git branch "development"
```
6.- Now we have to set the new branch as main 
```
$ git checkout "development"
```
7.- We will make a change to the README file

With the status command we can see the changes we just made 
```
$ git status
```
8.- To be able to save it in github we have to execute the add command 
```
$ git add .
```
And commit with the command: 
```
$ git commit -m "commit_name"
```
9.- Finally we will push to our github following the following command  and we will be able to visualize it in our github 
```
$ git push --set-upstream origin "development"
```
10.- Now we will create another branch called "features" and we will follow the same steps used previously 
```
$ git branch "features"
```
```
$ git checkout "features"
```
Make here a change to the README file
```
$ git status
```
```
$ git add .
```
```
$ git commit -m "commit_name"
```
```
$ git push --set-upstream origin "features"