# Introduction
Welcome in the very first lab of MICRO-315

# Part 1 - Integrated Development Environment (IDE)
Click on one the links accordingly to you computer's configuration
- 👉 [❖ Windows](https://github.com/epfl-mobots/MICRO-315-TPs-Student/wiki/Installing-the-IDE-%7C-%E2%9D%96-Windows)
- 👉 [🍎 MacOS]()
- 👉 [🐧 Linux]()

The IDE now freshly installed, let's start by quickly presenting IDE which we will use throuhought this whole semester.
- 👉 [🛠 Tools](https://github.com/epfl-mobots/MICRO-315-TPs-Student/wiki/IDE-%7C%F0%9F%9B%A0-Tools)
- 👉 [🗔 User Interface](https://github.com/epfl-mobots/MICRO-315-TPs-Student/wiki/IDE-%7C-%F0%9F%97%94-User-Interface)

# Part 2 - Presenting the EPuck2
- 👉 [Click here](https://github.com/epfl-mobots/MICRO-315-TPs-Student/wiki/EPuck2-%7C-Presenting-the-EPuck2)
## Demo program 1
- open in VSCode EPuck2 the folder under Workplace_EPuck2/Lib
- run the task `Make ST`
- go in the **Run and Debug** and click on `Start Debugging` OR press `F5`
- run the task `Run ST`

## Demo program 2
- still in the folder Workplace_EPuck2/Lib
- run the task `Make e-puck2_main-processor`
- go in the **Run and Debug** and click on `Start Debugging` OR press `F5`
- run the task `Run EPuckMonitor`

# Part 3 - Presenting Git
- 👉 [Click here](https://github.com/epfl-mobots/MICRO-315-TPs-Student/wiki/Git-Presenting-Git)
- take inspiration [here]https://rogerdudler.github.io/git-guide/)
## Exercise with git
Let's 

# Part 4 - Setting up your group TP's repository
- This part explains how to set up the github repository that you will BOTH be using during the labs
- It is very important to use the git tool
- Only ONE person needs to perform the initialization of the github repository, this person will have to follow the steps in Computer1's section
- The other person will have to follow the steps in Computer2's section
- ⚠ The two memnbers of the group must create github account if they do not own one
## Computer 1
- Clone the repository in the Workplace
  ```
  git clone https://github.com/epfl-mobots/MICRO-315-TPs-Student .../Workplace_EPuck2/TPs
  cd Workplace_EPuck2/TPs
  ```
- Let's check the already existing remotes and branches
  ```
  $ git remote -v
  origin        https://github.com/epfl-mobots/MICRO-315-TPs-Student (fetch)
  origin        https://github.com/epfl-mobots/MICRO-315-TPs-Student (push)
  ```
  - As we can see, there is one remote named **origin** pointing to the url of the cloned repository
  - However, you have no right to push (write) anything on this github repository
  - To do so, you have to connect this repository to your github repository
  - 💡 A **remote** is a version of repository stored elsewhere, usually on a server 
- Rename the **origin** remote into **upstream**
  ```
  $ git remote rename origin upstream
  $ git remote -v
  upstream      https://github.com/epfl-mobots/MICRO-315-TPs-Student (fetch)
  upstream      https://github.com/epfl-mobots/MICRO-315-TPs-Student (push)
  ```
- Create the github repository which will store your work's group during the labs
  - ⚠ Create ONLY ONE github repository per group
  - Click on `New Repository`
  ![]()
  - Name it as you wish, for instance **MICRO-315-TPs**
  ![]()
  - Add your workmate in the collaborator list
    - ![]()
    - your workmate will receive the invitation by e-mail
  - That's it !
  - 💡 Ignore github's tips on quick setup
- Add the remote, replace the github link with the one of your repo
  ```
  $ git remote add origin https://github.com/username/MICRO-315-TPs
  $ git remote -v
  origin          https://github.com/username/TPs (fetch)
  origin          https://github.com/username/TPs (push)
  upstream        https://github.com/epfl-mobots/MICRO-315-TPs-Student (fetch)
  upstream        https://github.com/epfl-mobots/MICRO-315-TPs-Student (push)
  ```
- Now push all those changes to your repo
  ```
  git push -u origin --all
  ```
- Checkout to TP1_Exercise branch and push the changes to your repo
  ```
  $ git checkout TP1_Exercise
  $ git push -u origin --all
  ```

## Computer 2
- Execute this steps only once the work on computer 1 is over
- Launch a terminal in the Workplace_EPuck2 directory
- Clone your workmate repository
  ```
  & git clone https://github.com/username/TPs
  ```
- Add the remote pointing to https://github.com/epfl-mobots/MICRO-315-TPs-Student
  ```
  & git remote add upstream https://github.com/epfl-mobots/MICRO-315-TPs-Student
  ```
- Checkout to TP1_Exercise branch
  ```
  $ git checkout TP1_Exercise
  ```

# Part 5 - STM32F4 Microcontroller and GPIO configuration
  
