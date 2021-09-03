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

**optional**
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
