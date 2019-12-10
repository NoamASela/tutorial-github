# Git Workshop
Lab 7: Using the Feature Branch Workflow

---

## Exercise


 - Browse to the github lab01 repository page:
```
https://github.com/NoamASela/github-lab01.git
```

 - Sign-in to github using your credentials
 - Clone the repository locally using the command / source tree:
```
$ git clone https://<PutNoamAmraniPersonalAccessToken>@github.com/NoamASela/github-lab01.git
```
```
ST: New Tab
ST: Clone
ST: Enter the URL and destination
ST: Clone
```

 - Create a feature branch for your changes (and move to the branch):
```
$ git checkout -b feature/<your-name>
```
```
ST: On the top menu: select Repository -> Branch (CTRL+SHIFT+B)
ST: Make sure you do that from the right branch (master is current branch)
ST: Name the branch feature/noama
```

 - Edit the README.md file adding a line with your name:
```
# <your-name>
```

 - Commit your changes locally:
```
$ git add -A
$ git commit -m "Added name <your-name>"
```
```
ST: On the left pane, go to Workspace: File Status
ST: Stage selected file
ST: In the comments, type "Added name <your-name>"
ST: Commit the changes
ST: On the left pane, go to History and view your commit
```

 - Push your changes to the remote repository (creating the branch in the remote repo):
```
$ git push -u origin feature/<your-name>
```

```
ST: On the upper ribbon, click 'Push'
ST: Select your branch to push and click 'Push'
```

 - create a new file with your firstname.lastname:
```
$ echo "." >> <firstname.lastname>

for example:
$ echo "." >> noam.amrani
```

 - Commit your changes locally:
```
$ git add -A
$ git commit -m "Added name <your-name>"
```
```
ST: On the left pane, go to Workspace: File Status
ST: Stage selected file
ST: In the comments, type "Added <your-name> file"
ST: Commit the changes
ST: On the left pane, go to History and view your commit
```

 - Push your changes to the remote repository (creating the branch in the remote repo):
```
$ git push -u origin feature/<your-name>
```
```
ST: On the upper ribbon, click 'Push'
ST: Select your branch to push and click 'Push'
```

 - Open a pull request using source tree or the URL provided from the push. 
```
 $ git push origin feature/noama
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 237 bytes | 237.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'userb' on GitHub by visiting:
remote:      https://github.com/NoamASela/github-lab01/pull/new/userb
remote:
To https://github.com/NoamASela/github-lab01.git
 * [new branch]      userb -> userb
```
```
ST: On the left pane, expand: Remotes -> origin -> feature
ST: Right click your branch and choose 'Create Pull Request'
``
 - Logout from GitHub
 

 - The Administrator will get notified and will merge your PR

## Tips

 - You will probably have to handle some conflicts merging your changes
