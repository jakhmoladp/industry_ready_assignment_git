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
a. status when files are not tracked:
![image](https://user-images.githubusercontent.com/54409180/194828660-9e92dc56-08d6-464b-aa44-005c61bbc2e7.png)

b. status when files is being tracked but changes not commited:
![image](https://user-images.githubusercontent.com/54409180/194828821-9877951a-6ad9-4ca0-b66b-25fb8ffea7f4.png)

c. status after committing the changes:
![image](https://user-images.githubusercontent.com/54409180/194829078-63272ead-8da5-4cbb-9913-65fc5bb48500.png)

