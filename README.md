```
vocstartsoft:~/environment $ ls -a
.  ..  .c9  README.md
vocstartsoft:~/environment $ cd ~/.ssh/
vocstartsoft:~/.ssh $ ll
lll: command not found
vocstartsoft:~/.ssh $ ls
authorized_keys
vocstartsoft:~/.ssh $ cd /home/ubuntu/environment
vocstartsoft:~/environment $ echo "# django-todo" >> README.md
vocstartsoft:~/environment $ git init
Initialized empty Git repository in /home/ubuntu/environment/.git/
vocstartsoft:~/environment (master) $ git add README.md
vocstartsoft:~/environment (master) $ git commit -m "first commit"
[master (root-commit) e9346ed] first commit
 Committer: Ubuntu <ubuntu@ip-172-31-38-109.ec2.internal>
Your name and email address were configured automatically based
    git config --global user.name "Your Name"
    git config --global user.email you@example.com

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 15 insertions(+)
 create mode 100644 README.md
vocstartsoft:~/environment (master) $ git remote add origin git@github.com:jessdevine/django-todo.git
vocstartsoft:~/environment (master) $ git config --global user.email jessica.devine@wpengine.com
vocstartsoft:~/environment (master) $ echo "# django-todo test" >> R
EADME.md
vocstartsoft:~/environment (master) $ git remote -v
origin  git@github.com:jessdevine/django-todo.git (fetch)
origin  git@github.com:jessdevine/django-todo.git (push)
vocstartsoft:~/environment (master) $ git commit -m "test"
On branch master
Changes not staged for commit:
        modified:   README.md

Untracked files:
        .c9/

no changes added to commit
vocstartsoft:~/environment (master) $ git add README.md 
vocstartsoft:~/environment (master) $ c^C
vocstartsoft:~/environment (master) $ git push -u origin master
The authenticity of host 'github.com (140.82.114.4)' can't be established.
RSA key fingerprint is SHA256:nThbg6kXUpJWGl7E1IGOCspRomTxdCARLviKw6E5SY8.
Are you sure you want to continue connecting (yes/no)? yes
Warning: Permanently added 'github.com,140.82.114.4' (RSA) to the list of known hosts.
git@github.com: Permission denied (publickey).
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
vocstartsoft:~/environment (master) $ echo "# django-todo test2" >> README.md     vocstartsoft:~/environment (master) $ git commit -m "test 2"                      
[master abf9d46] test 2
 1 file changed, 1 insertion(+)
vocstartsoft:~/environment (master) $ git status
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   README.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        .c9/

no changes added to commit (use "git add" and/or "git commit -a")
vocstartsoft:~/environment (master) $ git add README.md 
vocstartsoft:~/environment (master) $ git commit -m "test 3"                      
[master bde0054] test 3
 1 file changed, 1 insertion(+)
vocstartsoft:~/environment (master) $ git push -u origin master                   
git@github.com: Permission denied (publickey).
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
vocstartsoft:~/environment (master) $ 
```