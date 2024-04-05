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