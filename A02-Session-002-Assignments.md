**Session \- 02 \- Understanding GitHub**

1. Preparation  
   1. Open terminal and go to your home directory  
   2. Create a folder by name **workspace** below  
      1. This will be the folder in which you will do most of all your development  
      2. The name here is a suggestion.  
      3. You can choose any name of your choices like:  
         1. go  
         2. workspace\_go  
         3. code  
   3. Create a folder structure as shown below   
      1. In the document **sachin** as \<your git account name\>

2. Git Commands  
   1. **Step 01**  
      1. Open Github and login to your account  
      2. Create a git repo on your account by name **training**  
         1. Make sure to add **Readme** file  
      3. Open terminal and go to **sachin** folder  
      4. Clone your **training** repo here  
   2. **Step 02**  
      1. Create a branch by name **development** and checkout  
      2. Push this branch to Github
      pushed changes to development

   3. **Step 03**  
      1. Create a branch by name **my\_first\_branch** and checkout  
      2. Open the repository in code editor  
      3. Add your name, your college name, address in Readme file  
      4. Commit your change \- Add meaningful commit message  
      5. Push the branch to github  
      6. Go to github and raise a Pull Request with **development** as base branch  
      7. Get one of your team member to approve the pull request  
      8. Merge the PR \- (**test** release)

   4.  **Step 04**  
      1. Go to terminal and your repo  
      2. Open **commit graph** and understand how branches are related  
         1. Try to understand local branch and remote branch  
      3. Note down the commit id of all 3 branches in Readme file with appropriate description  
         1. main  
         2. development  
         3. my\_first\_branch  
      4. Ensure your local **development** is updated with latest merged code from github  
      5. After this update study the commit graph again and note down the commit id of 3 branches

   5. **Step 05**  
      1. Go to Github and create PR from **development** with **main** as base branch    
      2. Get PR Approved from team member  
      3. Merge the PR \- (**stage** release)  
      4. Open your repo in terminal  
         1. Study the commit graph  
      5. Update all 3 branches  
         1. Study commit graph again

***Note:*** 

* ***Commit Graph***  
  * *Going forward, make it a regular habit to review the **commit graph** at each step.*  
  * *This will help you better understand the structure and flow of changes in the codebase.*  
  * *After each prod release study all releases and their notes*  
* ***Release Processes***  
  * *The **release process** you are practicing is intended solely to provide you with exposure to the general workflow.*   
  * *Please note that in real-world projects, there will be additional steps such as **Build, Test, and Deployment**, which are **not included** in this exercise.*  
  6. **Step 06**  
     1. **Subtask-01**  
        1. Create a branch by name **feature\_01** from **development** and checkout  
        2. Add your favorite/inspiring quote in a file **quotes/first\_quote.md**  
        3. Commit the change  
     2. **Subtask-02**  
        1. Create a branch by name **feature\_02** from **development** and checkout  
        2. Choose one of JSON api response from your session 01 (say animals)  
        3. Add that json file under **interesting/animals.json**  
     3. **Subtask-03**  
        1. Push **feature\_02**  to Github and merge it to **development** using PR process  
     4. **Subtask-04**  
        1. Get latest update of development branch on your local system  
        2. Merge **development** into **feature\_01**  
        3. Raise PR on **feature\_01** to **development** and merge through PR process  
     5. **Subtask-05**  
        1. On Github, generate a release not from **main** branch with tag **v0.0.1**  
        2. Publish release \- (**prod** release)  
     6. **Subtask-06**  
        1. On your local repo, update all your local branches to be in-sync with remote branches  
        2. Fetch the latest tags from remote  
        3. Study the commit graph  
     7. **Subtask-07**  
        1. Using **feature\_02** branch, do test, stage and prod releases  
     8. **Subtask-08**  
        1. Study the commit graph   
        2. Update all local branches  
        3. Fetch all release tags  
        4. Study the commit graph

  7. **Step 07**  
     1. Add all your files from **Session-01** to **main** branch by going through all steps  
        1. Local branch \-\> PR to development \-\> PR to main \-\> Release

3. Git with team member  
   1. Pair up with a team member  
   2. Clone their repo in your system  
      1. You will be *Developer*  
      2. The repo owner will be *Reviewer*  
   3. Add your mentors to your repository, so that they can review your code  
   4. Repeat all steps from **Step-03** on each others repository  
      1. In each PR step, assign your team member(owner of repo) to review  
      2. Let the reviewer, give a review comment/suggestion  
      3. Reviewer \-\> Give creative review requests  
      4. Developer \-\> Work on the review feedback and re-request the review  
      5. Reviewer \-\> Ensure the review is addressed and only then merge the PR

**Final Instructions:**

1. Once you finish practicing on your repo, push all your code to “Training Repo” shared with you.  
2. Use one branch with your name as prefix  
   1. Under **Day-0**, create a folder by your name  
   2. Add your code/work.  
   3. Raise PR to development branch  
   4. Merge to development.  
   5. No need to merge to main and release flow.

**Additional Resources:**

1. [Linus Torvalds & git](https://www.youtube.com/watch?v=idLyobOhtO4)  
2. [Git through Images](https://dev.to/nopenoshishi/understanding-git-through-images-4an1)
