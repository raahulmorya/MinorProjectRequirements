## Differences between Git and GitHub

Git is a version control system that manages and keeps track of your code. GitHub, on the other hand, is a service that let you host, share, and manage your code files on the internet.

GitHub uses Git underneath, and lets you manage your Git repositories or folders easily on its platform.

So Git is the actual version control system and GitHub is the platform where you host your code.

## How to Start Using Git and GitHub

### Step 1 – Install Git
Preinstalled in Macs and Linux-based systems
Check Git installed in machine by typing `git version` in terminal  

![[Pasted image 20240405120505.png]]

### Step 2 – Create a GitHub Account.
### Step 3 – Connect your GitHub account to your Git account.
To set Git username, type this in terminal:

```shell
git config --global user.name "myusername"
```

To confirm Git username is correct, type this:

```shell
git config --global user.name
```
To set Git email, type this in terminal:

```shell
git config --global user.email "youremail@gmail.com"
```

To confirm Git email is correct, type this:

```shell
git config --global user.email
```
### Step 4 – Create and edit your code files locally
### Step 5 – Create a repository on GitHub
![[Pasted image 20240405121232.png]]
![[Pasted image 20240405121244.png]]
![[Pasted image 20240405121254.png]]
### Step 6 – Push your local code to GitHub
`echo "# sample-code" >> README.md`

`git init`

`git add .`

`git commit -m "first commit"`

`git branch -M main`

`git remote add origin https://github.com/segunajibola/sample-code.git`

`git push -u origin main`
Note that `git add README.md`  in the repository on GitHub. But here `git add .`, which is to let Git add all code files instead of the `README.md` file which will be created by `echo "# sample-code" >> README.md`. So if created other files in local folder, need to use `git add .` to add all files.

Take note that `git remote add origin [https://github.com/segunajibola/sample-code.git](https://github.com/segunajibola/sample-code.git)` will contain the link to own repository and it will have have the name of GitHub account.

## Common Git Commands to Know

They are many Git commands to use in the terminal, and that can get overwhelming. most popular ones first.

Here they are:

`git init` lets you initialize Git in your folder.

`git add [Readme.md](https://readme.md/)` lets you add the Readme file, while `git add .` lets you add all files in the present folder.

`git commit` stores the added files. Use `-m` for message followed by the actual message.

`git branch` creates a new branch which is a new version of the repository as it appears when added, and `-M` to move the name to `main`.

`git remote add origin` finally connects the local folder to the repository on GitHub. It is followed by the repository's link.

`git push -u origin main` pushes the code to GitHub. The `-u` flag creates a tracking reference for the branch, and `origin main` puts the code in the `main` branch.


