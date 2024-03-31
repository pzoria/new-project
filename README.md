#Start the task with the steps listed below.
#After successful execution, describe the instructions for developers in the Readme file.
#The result will be a public repository, a development branch, and an instruction file.

     #Create a new directory in your environment called "new-project".
        mkdir 'new-project'
     #Change to the "new-project" directory.
        cd 'new-project'
     #Initialize a new public Git repository inside the "new-project" directory.
        git init
     #Create a new file called "README.md" and add the opening text to it.
        vi README.md
     #Prepare the "README.md" file for the commit.
        git add README.md
     #Commit the changes to the repository with the commit message “init”.
        git commit -m "init"
        git push -u origin main
     #Create a new branch called "development" and switch to it.
        git chekout -b development
     #Add the instructions to the "README.md" file and prepare them for the commit.
        vi README.md
        git add README.md
     #Commit changes to the "development" branch with a commit message.
        git commit -m "new commit"
        git commit -u origin development
     #Merge changes from the "development" branch into the "main" branch.
        git chekout main
        git merge development
     #Check the status, make sure everything is up to date.
        git status
     #Commit the changes
        git commit -am "merge development branch into main"
