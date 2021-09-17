# Generate keys ssh from GNU/Linux for GitHub

## Instructions

1. Open console in your GNU/Linux system.


2. Run following command in your console:

```
ssh-keygen -t rsa -b 4096 -C "write your comment"
```

3. Press Enter to confirm file path

```
Enter file in which to save the key (/home/"your-system-user"/.ssh/id_rsa):
```

4. Create new password for your keys-ssh and press Enter

```
Enter passphrase (empty for no passphrase):
```

5. Type password again to confirm and press Enter

```
Enter same passphrase again: 
```

6. The result is:

```
Your identification has been saved in /home/"your-system-user"/.ssh/id_rsa
Your public key has been saved in /home/"your-system-user"/.ssh/id_rsa.pub
The key fingerprint is:
.....
....
...
```

7. Go to file path SSH (if your are in the root of the filesystem)

```
cd /home/"your-system-user"/.ssh
```

8. Open the example.txt file with your preferred text editor and copy to clipboard content, for example:
```
ssh-rsa hFkdmS+d5fn...........jds5Gjs4dfsJ.......
```

9. You go to your account on GitHub, settings and you click on the "SSH and GPG keys" option.

10. You click on the "New SSH key" button, paste the content of step number 8 on the "KEY" text field and you type a title.

11. You click on the "Add SSH key" to save the new key.


## Note!
* GIT credentials email must be the same as your GitHub account.
* _Config your user.name and user.email in GIT:_
```
git config --global user.name "type-user-name"
git config --global user.email "type-your-email"
```
