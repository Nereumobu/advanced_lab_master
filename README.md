# advanced_lab

******************************************* HOW TO START
-> Install Git with conda: 
    conda install -c anaconda git


******************************************** BRANCHES

-> Once installed you can create your branch with:
    git checkout -b <new branch name>
-> Working in a branch does not alter the documents in other branches. 
-> In other words one can work without stepping on each others toes.

-> In order to change branches one can use:
    git checkout <branch name>

-> Branches can be merged when they are not needed anymore. 
-> Suppose you are working in "mybranch" and create a new branch "hotfix" to solve some unrelated issue.
-> Then once this issue is solved one can merge hotfix into mybranch by:
    git checkout mybranch
    git merge hotfix

-> ATTENTION: Some times there will be issues with merging which derive from incompatible documents. 
-> EXAMPLE: If you have in hotfix you have edited documents from mybranch.
-> These have to be solved by hand.

********************************************************** ADDING, COMMITING AND PUSHING

-> When you make changes in your branch you have to add them using:
    git add <file name>
-> Or if you are removing files
    git rm <file name>
-> One can check which files have to be added with:
    git status
-> As you add files, you stage them for commitment. Once you have made all the changes you wanted
    during your working session you can commit them with:
    git commit -m <message with info about the commit>
-> This is akin as saving your work as you will always be able to go back to a previous commit.

-> How ever this changes are only made in your local repository in order to share this with the rest
    you have to use:
    git push

-> Similarly in order to get the changes that others have made you should use:
    git pull
+++++++++++++++++++++++++++++++++++++++++++++++ MORE

-> There is way more that you can do with git. For more information I like to check the git book:
    https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control
-> Chapter 2 and 3 are the ones I use the most.

-> Also the git cheat list in this directory is quite useful :)
