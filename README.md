# advanced_lab

********************************* HOW TO START *********************************

-> Install Git with conda: 
    conda install -c anaconda git


********************************* BRANCHES *********************************

-> Once installed you can create your branch with:

    git checkout -b <new branch name>
    
-> Working in a branch does not alter the documents in other branches.

-> In other words one can work without stepping on each others toes.

-> It is recommended that evrybody creates his own main branch, for example: "mainNereu", "mainTimo", "mainJacobo". And then work mainly in this branches, creating the necessary subbranches when needed. For example if I want to covert the txt files but I don't want to mess with my "mainNereu" branch I might do:
    git checkout mainNereu                  #I make sure that I am in my main working branch
    git checkout -b convertFilesNereu       #Create the branch where I will make the conversions

-> As seen before, in order to change branches one can use:
    git checkout <branch name>

-> Branches can be merged when they are not needed anymore. 
-> In the example from before if I have made sure that everything is working and want to have the converted files in my own working branch I can do:
    git checkout mainNereu          #Go to the branch I want to merge into
    git merge convertFilesNereu     #Merge the branches.

-> ATTENTION: Some times there will be issues with merging which derive from incompatible documents. These have to be solved by hand. Github will usually tell you what to do.

-> Once you are finished with a branch you can always delete it from the local repository with.
    git branch --delete <branch name>

-> Beware that in order to delete a branch from the remote, one has to do it by hand in the github webpage:

    https://github.com/Nereumobu/advanced_lab_master/branches/all

********************************* ADDING, COMMITING AND PUSHING *********************************

-> When you make changes in your branch you have to add them using:
    git add <file name>
-> Or if you are removing files
    git rm <file name>
-> One can check which files have to be added with:
    git status
-> This also tells us in what branch we are working.

-> As you add files, you stage them for commitment. Once you have made all the changes you wanted
    during your working session you can commit them with:
    git commit -m <message with info about the commit>
-> This is akin as saving your work as you will always be able to go back to a previous commit.

-> One may do this by first getting the list of all commits through
    git log 
-> Every commit has a hash code as an id, for example the one where I first added this Readme is "7b07e51a3e53725988fc4b38e65312a00fdb415d". With this one can return to a previous commit with:
    git checkout <commit id>

-> However these changes are only made in your local repository. In order to share this with the rest
    you have to use:
    git push

-> Similarly, in order to get the changes that others have made you should use:
    git pull
-> or:
    git fetch   #gets history of commits
    git merge   #merges this history into your repository

-> It is not always necessary to upload your new branches or commits to the GitHub remote. Sometimes it can be more comfortable to just mantain some branches as local branches in order to not clutter the remote, however this depends on personal preference and of course one should do whatever feels more natural for himself.

+++++++++++++++++++++++++++++++   MORE +++++++++++++++++++++++++++++++ 

-> There is way more that you can do with git. For more information I like to check the git book:
    https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control
-> Chapter 2 and 3 are the ones I use the most.

-> Also the git cheat list in this directory is quite useful.



-> Anyways if you get anything wrong (as I usually do), most of the time Git will tell you what to do :)
-> And if not a google search will surely do haha
