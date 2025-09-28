# git_command 123
 ---
[sintax markdown complete](https://chatgpt.com/share/68d58acb-45d4-8010-bff7-a1d500bfec28)
---
## git config
>  **set user.name & user.email**
```bash
git config --global user.name "your name"
git config --global user.email "your email"
```
  ---
  > **set default branch**
  ```bash
  git config --global init.defaultBranch main/master
  ```
  ---
  > **set code editor**
  ```bash
  git config --global core.editor "nano"
  ```
  --- 
> **viewing your configuration**
>>  ```bash
>>   git config --list
>>    ```
>>    ```bash
>>    git config user.name
>>    ```
  --- 
> **unseting**
>> ```bash
>> git config --global --unset 
>> ```
  --- 

## git commit
### **commit staged changed with message**
```bash
git commit -m "message"
```
### **commit all tracked changes (skip staging)**
```bash
git commit -a -m "message"
```
### **see commit history**
  ```bash
  git log
  git log --oneline # for shorter view 
  git --stat # to see which file changed in each commit
  ```
### **troubleshooting common commit mistakes**
+ forgot to stage a file ?
 ```bash
 git commit --amend
 ```
+ typo in your commit message?
```bash
git commit -amend -m "corrected message"
```
+ accidentally commited the wrong file 
```bash
git reset --soft HEAD~1  
```
## git branch
### **membuat dan mengelola branch lokal**
+ see list branch 
```bash
git branch
```
+ membuat branch baru
```bash
git branch nama-branch 
```
+ Beralih ke branch lain
```bash
git checkout nama-branch
git switch nama-branch
```
+ Membuat branch baru dan beralih ke branch tersebut
```bash
git checkout -b nama-branch
```
## Common git merge Options
+ git merge - Merge a branch into your current branch
+ git merge --no-ff - Always create a merge commit
+ git merge --squash - Combine changes into a single commit
+ git merge --abort - Abort a merge in progress