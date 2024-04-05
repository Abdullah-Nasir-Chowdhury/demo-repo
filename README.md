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
`Enter file in which to save teh key(/Users/..../id_rsa): testkey` </br>
`Enter passphrase (empty for no passphrase): [Enter]`
</br>