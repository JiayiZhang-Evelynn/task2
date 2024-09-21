The task2 link is

https://github.com/JiayiZhang-Evelynn/task2.git


In my terminal

mkdir task2  #create the folder

cd task2

git init #Initialize a Git repository

nano README.md

###Add “This is a readme file!” to the file

git add README.md

git commit -m "Added README.md with initial content"


<img width="545" alt="WeChat72cc8a9c06b2f619beeab2b3bb27b041" src="https://github.com/user-attachments/assets/385526c2-f8f8-4d95-8a31-64926145bd0b">


![5241726884511_ pic](https://github.com/user-attachments/assets/7f6fe929-94b4-423f-90e2-91081e750997)

![5261726885277_ pic](https://github.com/user-attachments/assets/18634e65-263a-4555-82de-f612d4663e83)
Then, create an empty repository on GitHub

Go to GitHub and create a new empty repository.

After the repository is created, copy the URL of the repository.

![5251726884679_ pic](https://github.com/user-attachments/assets/16972d73-80c8-4a70-bab9-ef83343b16a9)

Modify the README.md on GitHub:

"This is a remote readme file!"

Commit the changes directly to the main branch.

Open the README.md file locally and change the text to:"This is a local readme file!"

Commit and push the local changes:

git add README.md
git commit -m "Updated README.md to local version"
git push

###encounter a merge conflict since the content of the README.md file is different locally and on GitHub.

The file contain this:
<<<<<<< HEAD
This is a local readme file!
=======
This is a remote readme file!
>>>>>>> origin/main

![5311726886225_ pic](https://github.com/user-attachments/assets/6a6d597d-827c-4f91-87b9-590b6ec18efa)

###Add and commit the merge resolution

git add README.md

git commit -m "Resolved merge conflict in README.md"

git push origin main


![5321726886518_ pic](https://github.com/user-attachments/assets/66535644-b009-44df-91d4-5755fbdf2ddb)


Finally, both your local and remote repositories will have the same content in README.md:
"This is a readme file!"



GitHub Flow: Adding a new feature
Go to the GitHub repository and create an issue with the title "Making feature 1!".

###Create a new branch locally

###Create and edit the file FEATURE1.md:"This is feature 1!" 

git add FEATURE1.md

git commit -m "Added FEATURE1.md"

![5331726887056_ pic](https://github.com/user-attachments/assets/43b51707-c2fa-4ce5-b32e-f749cf27f3ad)


###Push the feature1 branch to GitHub:git push origin feature1

###Go to GitHub, and open a pull request to merge the feature1 branch into main.
###Approve and merge the pull request on GitHub.

![5341726887440_ pic](https://github.com/user-attachments/assets/7effb8af-2418-4059-ad2c-c3082385ffc9)

![5351726887452_ pic](https://github.com/user-attachments/assets/7c93ea95-f13c-4442-bf44-1e9f5962d8c2)

###After the merge is successful, close the "Making feature 1!" issue.


![5371726887559_ pic](https://github.com/user-attachments/assets/f98241cb-a3ec-47c3-be84-e839f0446dfc)


##Pull the latest changes to the local main branch:

git checkout main
git pull origin main
<img width="529" alt="WeChat21615891c6ebf907c37fba415dce45e5" src="https://github.com/user-attachments/assets/b1d5e2c2-83e1-4ed1-8a8d-e8b892d3a685">
