# Git
When you were doing all of those commands to get minetest and MineClone, that was git. In MineClone we use git to make commits and file system management.
To get started:
1. On the terminal or command prompt, enter your MineClone world.
2. If you have a fork, that should be the mineclone repository you should clone, not the main repository. As a beginner, it is recommended (And basically mandatory that you obtain a fork)
3. Type `git remote add upstream <main mineclone repository git>` in the command line or terminal. (Replace the "<main mineclone repository git>" with either https://git.minetest.land/MineClone2/MineClone2.git or https://git.minetest.land/MineClone5/MineClone5.git)
4. Type `git config --global user.name "<username>"`. Replace "<username>" with your MeseHub username.
5. Type `git config --global user.email "<email@email.com>"`. Replace "<email@email.com>" with the email you used to register with MeseHub.

That is how you setup your local git. Now its time to create your changes.
1. Create a new branch
    `git branch <branchname>`
    `git checkout <branchname>`
2. Create your changes.
3. To make a commit, first you need to stage your changes to be commited.
    
    a. `git add <file name>` will add a single changed file.
    
    b. `git add .` will stage all of the changed files.
    
    c. `git commit -m "<Commit name/description>"` will create the commit. Be sure to replace "<Commit name/description>" with a description of what your commit changes.
    
    d. To push these changes to your remote fork (I.e. Mesehub), `git push origin/<branchname>` where branchname is the branch you are making changes on. Use the username and password you provided when you registered for a Mesehub account.

4. If you are ready to merge your changes to the main repository, you need to create a Pull Request (PR).
    
    a. Go to the Mesehub Website.
    
    b. Go to your fork repository webpage.
  
    c. Open the branch you made your changes on.
  
    ![branch-dropdown](https://raw.githubusercontent.com/PrairieAstronomer/MineClone/gh-pages/mesehub_branches_list.png)
  
    d. Create a pull request by clicking the pull request button next to the branches dropdown list.
  
    ![pull request button](https://raw.githubusercontent.com/PrairieAstronomer/MineClone/gh-pages/pull_request_button.png)
  
    e. Use a descriptive title and desciption when creating your pull request.
  
    f. If your pull request is a work in progress, put `WIP:` at the beginnging of the title.
