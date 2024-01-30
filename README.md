# How to make a repository
- After you create a directory, finish your initial project "optional" and save it, you **initialize** your git repository in git bash using the command below:
	```git
		git init
	```
- Then, you should **stage** your repo using the command:
	```git
		git add . // you can put the file you want instead of dot
	```
- Now, you are ready to make your first `commit` and you should write a suitable message as below:
	```git
		git commit -m "Initial commit"
	```
- Instead of staging and committing your file you can make them in **one step**, but it is better to stage the file first till you make sure of the stability of new version and this it is:
	```git
		git commit -am "Initial commit"
	```
	## Now, you have a repository, and we want to upload it to [GitHub](https://github.com/), let's see how we can do this:
1. create a repository in your GitHub account and select which files you want it to prepare itself.
2. You have to connect your repository with GitHub repository by the command without quotes:
	```git
		git remote add 'Remote-name' 'The link of your repo'
	```
	> We will use https method but you can see how we can use ssh key when you are contributing in the repository with other people.
3. Rename the master branch with `main` as it appears in GitHub as below:
	```git
		git branch -M main
	```
4. Now you can push your repository using the command without quotes:
	```git
		git push -u 'Remote-name' main
	```
5. The OS will ask you to enter your GitHub account credentials to proceed your request and congratulations you now have a repository on GitHub.
