# Git and Github
Below tasks have been performed for **assignment#1 Git and Github tutorials** which is part of **"Industry Ready Data Science Projects"**, a course offered by www.ineuron.ai. 

Refer below link for assignment details:
https://github.com/Project-Neurons/Industry-Ready-Projects-Tasks/blob/main/Git_&_Docker/Assignment-1.md


## Task 1
Demonstrate minimum 15 basic Git command with explanation and screenshot.

### Solution:
#### 1. Initialize git in local machine
This command converts the local folder into git repository.
```
git init
```
![image](https://user-images.githubusercontent.com/54409180/194898129-6613ce90-4f90-4e04-b116-4d8e458d1d61.png)

#### 2. Configure user details
'config' command can be used for setting multiple configurations. In this step we are configuring the name and email id of user who is performing the operations in the git. 
```
git config user.name = devendra_jakhmola
git config user.email = devjakhmola1990@gmail.com
```
![image](https://user-images.githubusercontent.com/54409180/194898231-69665e1c-ff21-49c6-a02f-7a56c2eed210.png)
![image](https://user-images.githubusercontent.com/54409180/194898341-3fde9ff1-26f8-495d-be75-fbf1a8dce5e9.png)

#### 3. Track files
'add' command is used to place changes in the working directory to git staging area. Before committing a change, we must add it to the staging area.
```
git add .
```
![image](https://user-images.githubusercontent.com/54409180/194899072-43814961-9c54-4ff8-ba79-ed94500c4ee5.png)

#### 4. Add files to Staging Area
'commit' command tells the git to store the final changes. Git maintains the history of each commit which makes it is easy to rollback to any previous commit whenever required.
```
git commit -m "first commit"
```
![image](https://user-images.githubusercontent.com/54409180/194900392-1ae7ae1f-8184-42b0-905c-a3fdb6b069c5.png)


#### 5. Rename 'master' to 'main'
When we want to publish changes from local git repo to a github repo, we should ensure that the root folder alias are same in git and github. By default, the root folder in github is 'main' while git has 'master'. We run below command to rename 'master' to 'main'. 
```
git remote -M main
```
![image](https://user-images.githubusercontent.com/54409180/194901490-e7adc50d-d476-4c6e-9b10-d393ab966c65.png)

#### 6. Create a remote for Github repo
To connect local git repo to git hub repo, we have to create a 'remote' pointing to github repository. In below command we are adding a remote for github repository and given it an alias 'origin'. 
```
git remote add origin https://github.com/jakhmoladp/sample_repo.git
```
![image](https://user-images.githubusercontent.com/54409180/194906552-71bb03f1-41a9-4701-915c-57a5c7de316c.png)

#### 7. Push changes from local machine to github repo
In below command, we are now pushing the committed changes from local repository (main branch) to github repository via remote (origin) we created in previous step.
```
git push -u origin main
```
![image](https://user-images.githubusercontent.com/54409180/194906794-360621a6-8aee-4f99-9ef3-42d86093207c.png)

#### 8. Create and activate a branch
Git allows the developers to create copy of main repository, make changes in the copy and easily merge their changes to the parent repository without too much efforts.
These copies are called 'branches' in git. Developers can create branches from last working code and perform their changes, test them and merge them to parent branch. 
This allows multiple developers to collaborate easily. 

In below command we are creating a branch named 'dev' and then switch to it. Changes done in this branch are limited to the 'dev' branch only, until he/she merges the changes with main branch.
```
git checkout -b dev
```
![image](https://user-images.githubusercontent.com/54409180/194906914-fca1e8db-82b3-42aa-95c6-e6b61c663b0c.png)

#### 9. Merge changes in branch to main
Make some changes in the files and merge the changes to 'main' branch.
```
git checkout main
git merge dev
```
![image](https://user-images.githubusercontent.com/54409180/194907537-48f7df6d-0782-4838-8127-08d04fe35ae6.png)

#### 10. Remove a file
```
# Remove a previously created document
git rm "15 commands.docx"
```
![image](https://user-images.githubusercontent.com/54409180/194907730-ec399b0b-7081-47bf-881b-32fc03935ca8.png)

#### 11. Clone github repo to local machine
'cloning' allows downloading a github repository into local machine.
```
# Create a folder in local machine.
# cd the folder and run below mentioned clone command.
git clone https://github.com/Project-Neurons/Industry-Ready-Projects-Tasks.git
```
![image](https://user-images.githubusercontent.com/54409180/194907861-25e92bcf-19ae-4643-931a-920dfcae991e.png)

#### 12. Check the list of untracked, unstaged or uncommited changes
```
git status
```
![image](https://user-images.githubusercontent.com/54409180/194908121-a2ccdcfa-9e1e-4dde-9e35-957d73eedc42.png)

#### 13. Rollback commit
As git saves the history of changes through commits, we can always go back to the previous commits.

a. Add a new line in app.py file:

![image](https://user-images.githubusercontent.com/54409180/194831390-f24418a9-189e-433a-bf20-b232844168c3.png)

b. Add and commit the change:

![image](https://user-images.githubusercontent.com/54409180/194908330-880df542-8736-48d0-b109-ab7fdef6f04c.png)
![image](https://user-images.githubusercontent.com/54409180/194831610-f2bc3da0-91bb-40e5-bcb0-d674466ed84d.png)

c. Rollback the last commit:
```
# Remove the last commit to tracking area
git reset HEAD~1
```

After running the reset command, it will show the last changes as not staged for commit.
![image](https://user-images.githubusercontent.com/54409180/194908709-129f8009-3b55-4a6d-9201-9301f4b1b328.png)

#### 14. Check git logs
This command shows the list of all commits. Use this to see the commit history and id of specific commit. It also shows the pointer to the current head.
```
git log
```
![image](https://user-images.githubusercontent.com/54409180/194832578-20eb3a8a-3bac-4790-b45b-04a00d1e0c40.png)

#### 15. Create Stashes
Git stash is a built-in command with the distributed Version control tool in Git that locally stores all the most recent changes in a workspace and resets the state of the workspace to the prior commit state.
```
git stash 
git stash apply
```
![image](https://user-images.githubusercontent.com/54409180/194909040-6a466316-2ef6-4678-853d-771094ad7578.png)

----------------------------------------------------------------------------------------------------------------
## Task 2
Consider that you want to start an open-source project in your organization. Perform all the standard operation to create a repository with minimal permision for all the users. It should contain.
1. Proper open source structure
2. Proper Readme
3. Add 2 collaborator
4. Host GitHub Pages using settings (Designed to host your personal, organization, or project pages from a GitHub repository)

### Solution:
#### 1. Open source project structure has been created
```
https://github.com/jakhmoladp/git_project_structure.git
```
![image](https://user-images.githubusercontent.com/54409180/195248457-840374e8-0534-4d94-853f-4ac2d66fc48c.png)

#### 2. Read me file added:

![image](https://user-images.githubusercontent.com/54409180/195248226-70a90c9f-088b-43c7-a2b0-3258adf0bfd1.png)
![image](https://user-images.githubusercontent.com/54409180/195248263-849877a1-3a7a-4c17-aa76-5f8f72d90e96.png)
![image](https://user-images.githubusercontent.com/54409180/195248291-cab70264-4e37-4c2b-b434-65200765fb52.png)

#### 3. Two Collaborators have been added
![image](https://user-images.githubusercontent.com/54409180/195248589-a061c1fa-a82f-4571-bd3b-bddd8bbe3ae3.png)

#### 4. Host GitHub Pages using settings
![image](https://user-images.githubusercontent.com/54409180/195250687-d45a56ec-f9b7-4e07-b307-44890066321e.png)

![image](https://user-images.githubusercontent.com/54409180/195250767-dbf2e3b2-e5d2-4c0e-8fa2-11fea69e419d.png)

------------------------------------------------------------------------------------------------------------------
## Task 3
- Create a Issue in your github repository.
- Raise a pull request.
- Merge A pull request.
- Reject a pull request with proper comments.
- Add a Dependabot alerts in your github.(for above cases)
- Stash changes
- Create a release your package
- Setup a Projects Board for your project.
