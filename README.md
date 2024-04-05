# Demo

Demo for GitHub and Git

## What is it about?

Check out the text file.

## Brief description:
Follow the following steps
### Create SSH Key:
To clone the repository with the write permission, you need to prove to github that you are the owner of your account. For that you need the SSH key.
So you have to connect your local machine to your github account somehow. The way this is done is by using SSH keys. </br>
You need to start by generating a key locally using the `ssh-keygen` command. </br> 
Then  you specify the type of encryption, using `-t` to denote type and `rsa` as the encryption. </br>
Then you add the strength of encryption. For instance `-b 4096` </br>
And at the end you need to include your github email address. `-C "[your_github_email_address]"` </br>
It should like this: <b>`ssh-keygen -t rsa -b 4096 -C "email@example.com"`</b>
</br>

You will then be asked to enter the file in which you wish to save the key, either press Enter or provide a file name, the file doesn't have to be a pre-existing file, like you can use the name [testkey], without the brackets or using quotes or anything, just type the name, the file will automatically be generated. I pressed enter.
Next you will need to provide a passphrase, you could provide one or press enter(no passphrase). And your key will be generated. </br>
`Enter file in which to save the key (C:\Users\HP/.ssh/id_rsa): testkey` </br>
`Enter passphrase (empty for no passphrase): [Enter]`
</br>

#### Find your testkey:
Your test key might be in the previous folder. So, go back to the folder, and:
type `ls` in the command terminal 

</br>
To print out your testkey, type: `cat testkey.pub`
It starts with ssh-rsa and ends with your email.
</br>

To print out your private testkey, type: `cat testkey`

#### Copy your SSH Key
Do not use `ctrl+c` or `cmd+c` </br>
use `pbcopy </testkey.pub>` on Windows
use `pbcopy <~/testkey.pub>` on Mac

#### GitHub SSH Key setup
Go to your SSH and GPG keys in your github account
Create New ssh key, give whatever title you want, and add SSH key.
The only thing left to do, is to make sure your local git command line interface knows about the key you just generated.

#### Adding your SSH key to the ssh-agent
Next follow the steps in this like:
</br>
![https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent#adding-your-ssh-key-to-the-ssh-agent]

## git clone:
To clone your repo, head over to the repo, and find the one with the ssh key, copy it, and type `git clone [the_copied_ssh_clone]` in the terminal

## ls:
Using `ls` you can find the folders in your cloned folder.

## ls -Force:
Using `ls -Force` you can find the hidden folders in your cloned repository.

## Making changes to the repo:
You can now make changes to the repo in your local machine and see what changes you made using `git status` it will show you the modified and untracked files

## git status
shows you the modified and untracked files

## git add .
adds all the modified and untracked files for commiting

## git add [file_name]
adds only the file_name for commiting 

## git commit -m ["message"] -m ["description"]
commit for pushing the added files to your github

## git push
push the files to the repo

## git branch --list
to check the list of your branches use `git branch --list`

## git push origin main
pushes to the origin/main branch
if you see that you have master the main branch: `git push origin master`
else `git push origin main`

# How to upload from your local machine to github?

