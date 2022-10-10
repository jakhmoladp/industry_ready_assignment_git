# Git and Github
Below tasks have been performed as part of assignment#1 Git and Github tutorials. 

Refer below link for assignment details:
https://github.com/Project-Neurons/Industry-Ready-Projects-Tasks/blob/main/Git_&_Docker/Assignment-1.md


## Task 1
Demonstrate minimum 15 basic Git command with explanation and screenshot.

## Solution:
### 1. Initialize git in local machine
```
git init
```
![image](https://user-images.githubusercontent.com/54409180/194827184-3a949ac2-ba72-4eeb-8374-e72a30ba09f0.png)

### 2. Configure user details
```
git config user.name = devendra_jakhmola
git config user.email = devjakhmola1990@gmail.com
```
![02  git config user](https://user-images.githubusercontent.com/54409180/194824463-e47990f7-966b-408f-99d3-336e3340c3e6.JPG)

### 3. Track files
```
git add .
```
![03  git add](https://user-images.githubusercontent.com/54409180/194825007-0d1d738a-3559-49de-abf9-38b3c6726150.JPG)

### 4. Add files to Staging Area
```
git commit -m "first commit"
```
![05  git commit](https://user-images.githubusercontent.com/54409180/194825150-084abf50-69c2-4d7c-b96a-fd93efa034d3.JPG)

### 5. Rename 'master' to 'main'
```
git remote -M main
```
![07  rename master to main](https://user-images.githubusercontent.com/54409180/194825758-1e290859-f22f-468b-9722-f452a2bd0e3b.JPG)

### 6. Create a remote for Github repo
```
git add remote origin https://github.com/jakhmoladp/industry_ready_assignment_git.git
```
![07  rename master to main](https://user-images.githubusercontent.com/54409180/194825758-1e290859-f22f-468b-9722-f452a2bd0e3b.JPG)

### 7. Push changes from local machine to github repo
```
git push origin main
```
![07  rename master to main](https://user-images.githubusercontent.com/54409180/194825758-1e290859-f22f-468b-9722-f452a2bd0e3b.JPG)

### 8. Create and activate a branch
```
git checkout -b dev
```
![10  create branch](https://user-images.githubusercontent.com/54409180/194825525-04002b14-3d67-4a5a-bc71-d071fc6ac4ed.JPG)

### 9. Merge changes in branch to main
```
git checkout main
git merge dev
```
![11  merge command](https://user-images.githubusercontent.com/54409180/194826917-a0f99c3d-1964-4e90-bf66-fcd1684daeb6.JPG)

### 10. Remove a file
```
# Remove a previously created document
git rm "15 commands.docx"
```
![image](https://user-images.githubusercontent.com/54409180/194824188-5fb5c5a9-d241-4b83-82c9-c507ddaeaf24.png)

### 11. Clone github repo to local machine
```
# Create a folder in local machine.
# cd the folder and run below mentioned clone command.
git clone https://github.com/Project-Neurons/Industry-Ready-Projects-Tasks.git
```
![image](https://user-images.githubusercontent.com/54409180/194828209-6c21040f-8ecf-47f7-99ab-2e1d2c3309e3.png)

### 12. Check the list of untracked, unstaged or uncommited changes
```
git status
```
![image](https://user-images.githubusercontent.com/54409180/194828660-9e92dc56-08d6-464b-aa44-005c61bbc2e7.png)
![image](https://user-images.githubusercontent.com/54409180/194829760-509ee65d-d4db-4f85-8662-f58303b29e1d.png)
![image](https://user-images.githubusercontent.com/54409180/194829870-6820c0c7-cbda-43c1-bbff-f385eb98e3a9.png)

### 13. Rollback commit

a. Add a new line in app.py file:

![image](https://user-images.githubusercontent.com/54409180/194831390-f24418a9-189e-433a-bf20-b232844168c3.png)

b. Add and commit the change:

![image](https://user-images.githubusercontent.com/54409180/194831567-7301edc4-f3d0-4a15-ad83-2ee92c201ea6.png)
![image](https://user-images.githubusercontent.com/54409180/194831610-f2bc3da0-91bb-40e5-bcb0-d674466ed84d.png)

c. Rollback the last commit:
```
# Remove the last commit to tracking area
git reset HEAD~1
```

After running the reset command, it will show the last changes as not staged for commit.
![image](https://user-images.githubusercontent.com/54409180/194831888-d916d1d4-1ce4-43df-97f5-b63d56a552a7.png)

### 14. Check git logs
This command shows the list of all commits. Use this to see the commit history and id of specific commit. It also shows the pointer to the current head.
```
git log
```
![image](https://user-images.githubusercontent.com/54409180/194832578-20eb3a8a-3bac-4790-b45b-04a00d1e0c40.png)

### 15. Create Stashes
```
git stash 
git stash apply
```
![image](https://user-images.githubusercontent.com/54409180/194833942-23c2d824-6927-4655-af2b-83d91d7eeb36.png)
