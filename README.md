# How-to-connect-Atom-and-Github
This repository essentially includes the simple steps to connect Atom and GitHub in correct order. Please suggest edits shall there be any.


__*The steps:*__[0]

1. Create a GitHub account and log-in.

2. Go to github.atom.io/login/. Re-enter password.
	Grant the access permission for atom.
	Copy the token.

3. Open Atom. From the bottom right corner, click 'GitHub'. Enter the copied token, there.

4. Create a local folder for the project.

4. Download and install Git.
	Open GitBash or CMD in the local folder for the project that you've just created, (and where you want to make a commit.)
	Type
		git config --global user.email "type_your_email_here"
	Press Enter and type:
		git config --global user.name "type_your_name_here"
	And press Enter.
(This way, it recognizes that it's you.)

5. Create a repository on Github.com.

6. In atom, press Ctrl + Shift + P. Search for Git Clone and open it.

7. Open the repository you created from github.com. Copy its HTTPS url, and paste it in the GitClone pop-up in Atom. Do not close the tab on web browser, yet.

8. Copy the path of local folder that you created in step 4, and paste it in the GitClone pop-up in Atom.

9. In the bottom right corner of Atom, click 'Fetch'. Open web browser and switch to the repository tab (or basically open github.com).
After a few seconds, you will see a pop-up asking to login. Login there. Do not choose the open for pasting token, because you would have to open "github.atom.io/login/" again, and as soon as you click anywhere else on the screen, the log-in pop-up would vanish.

# If you already have a project created locally:
In case you have already created all the files for your project locally, proceed the same way until step 8.

After performing step 8, upload all the files from your original local project folder to the remote repository on GitHub, manually (i.e. in the way you would usually upload any file online.)

Now, proceed to step 9.

# Important Points:

1. While 'commiting' files from the staged area, make sure the 'message' box isn't empty.
  
2. To delete a local or remote git branch, refer this link[1]. Avoid creating unwanted branches.
    
3. To unlink a local directory from github, delete the .git folder.[2]

Open GitBash and use this command:[3]

`git rm -rf .git`

4. There is no need to unlink an unwanted local directory from GitHub, simply delete the local folder.[4]


# Useful Command Line Commands:

* Create a new repository on the command line:
```
echo "# repository-name" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/username/repository-name.git
git push -u origin main
```
* Push an existing repository from the command line
```
git remote add origin https://github.com/username/repository-name.git
git branch -M main
git push -u origin main
```
# References
[0] https://youtu.be/6HsZMl-qV5k

[1] https://linuxize.com/post/how-to-delete-local-and-remote-git-branch/

[2] https://discuss.atom.io/t/delete-root-directory-and-unlink-directory-to-github-repository/44355

[3] https://teamtreehouse.com/community/how-to-remove-git-from-the-current-folder

[4] https://stackoverflow.com/questions/5667106/how-to-delete-or-change-directory-of-a-cloned-git-repository-on-a-local-computer

