# nova_award_2021

## Overall Requirements
- access to a computer
- access to a method to install software if needed

## Optional Requirements (makes things easier)
- Github account
- ssh key

### sign up for github instructions
1. Navigate your browser to https://github.com/signup
2. enter the information asked for at the prompt:
> -  user email
> -  user password
> -  username
3. open email account used during sign-up and click the link in the verification email

### ssh key generation
1. Open a command prompt by doing one of the following:
>  - win key + r and enter `cmd.exe`
>  - right-click the start button and select command or powershell
>  - open search and type cmd
2. At the prompt type in the command `ssh-keygen` and press enter
3. Press enter to set the filename as the default *id_rsa* or enter a separate filename if wanted
4. Enter a passphrase (something you can remember because you cannot change or retrieve it)
5. The ssh key is generated and an ascii image is displayed on completion. You can close the command window now.
6. The private and public keys are located in `C:\Users\<USERNAME>\.ssh` where USERNAME is your windows user name

### add ssh key to your github account
1. Log in to your Github account
2. In the top right corner click on your account avatar
3. Go to `Settings`
4. On the left side navigation list, select `SSH and GPG Keys`
5. Above the SSH Key dialog, click `New SSH Key`
7. Name your key with an easily recognizable name
8. Paste the entire contents of the *id_rsa.pub* file you created above
9. Click `Add SSH Key`

### To open the id_rsa.pub file
1. Open _File Explorer_
2. Navigate to `C:\Users\<username>\.ssh`
3. Right-click the *id_rsa.pub* file
4. Select _Open with_ and pick **notepad**
  - this is the text to paste into Github to add to your profile

### NEXT STEPS
1. Send me an email with your Github username or email address
2. I will add you as an authorized developer on the repository
3. Clone a local copy of the repository to your hard drive
4. Create a new branch with your first initial and last name  

#### to create a branch on a repo
1. Open a terminal
2. `cd` to your repository directory
  - I store mine in a new dir in my home folder @ `%HomePath%\git`
  - This repository would then be `%HomePath\git\nova_award_2021`
3. type `git checkout -b <branchname>` and press enter
  - for example: `git checkout -b jvoss` would create a new branch named **jvoss**
4. type `git add --all`
  - this tells git to add all of the current files to the branch
5. type `git commit -a -m "commit message"`
  - this tells git to commit all of the changes
  - the commit message can be anything you want it to be - make it easy to understand
6. type `git push`
  - if this is the first time pushing, you need to type `git push --set-upstream origin <branchname>` to tell git which branch you will be pushing to
  - you only have to run this once -- afterwards git knows which branch to push to until you make a new one
7. your branch is now visible in Github and can be cloned by anyone else
