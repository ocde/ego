ego
===
about junqing.

克隆版本库

git clone https://github.com/ocde/ego.git


git clone git@github.com:ocde/ego.git


need config following

~~~~~~~~~~~~~~
Step 1: Check for SSH keys
cd ~/.ssh# Checks to see if there is a directory named ".ssh" in your user directory
If it says "No such file or directory" skip to step 3

Step 3: Generate a new SSH key
ssh-keygen -t rsa -C "your_email@youremail.com"# Creates a new ssh key using the provided email
# Generating public/private rsa key pair.
# Enter file in which to save the key (/Users/you/.ssh/id_rsa): [Press enter]

Step 4: Add your SSH key to GitHub
copy ~/.ssh/id_rsa.pub#   to  https://github.com/settings/ssh

ssh -T git@github.com# Attempts to ssh to github

You may see this warning:
# The authenticity of host 'github.com (207.97.227.239)' can't be established.
# RSA key fingerprint is 16:27:ac:a5:76:28:2d:36:63:1b:56:4d:eb:df:a6:48.
# Are you sure you want to continue connecting (yes/no)?

Don't worry, this is supposed to happen. Verify that the fingerprint matches the one here and type "yes".
# Hi username! You've successfully authenticated, but GitHub does not
# provide shell access.

If that username is correct, you've successfully set up your SSH key. Don't worry about the shell access thing, you don't want that anyway.


