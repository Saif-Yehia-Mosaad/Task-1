
E:\>git clone https://github.com/Saif-Yehia-Mosaad/Task-1
Cloning into 'Task-1'...
warning: You appear to have cloned an empty repository.

E:\>

E:\>cd Task-1

E:\Task-1>git checkout -b feature2
Switched to a new branch 'feature2'

E:\Task-1>echo Hello DevOps Feature2 > index.html

E:\Task-1>dir
 Volume in drive E has no label.
 Volume Serial Number is 340F-DD17

 Directory of E:\Task-1

03/08/2026  04:01 AM    <DIR>          .
03/08/2026  04:01 AM                24 index.html
               1 File(s)             24 bytes
               1 Dir(s)  110,297,915,392 bytes free

E:\Task-1>git add index.html

E:\Task-1>git status
On branch feature2

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   index.html


E:\Task-1>git commit -m "Add new line to index.html"
[feature2 (root-commit) 01c5a6d] Add new line to index.html
 1 file changed, 1 insertion(+)
 create mode 100644 index.html

E:\Task-1>git push origin feature2
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 256 bytes | 256.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/Saif-Yehia-Mosaad/Task-1
 * [new branch]      feature2 -> feature2

E:\Task-1>git checkout main
error: pathspec 'main' did not match any file(s) known to git

E:\Task-1>git merge feature2
Already up to date.

E:\Task-1>git push origin main
error: src refspec main does not match any
error: failed to push some refs to 'https://github.com/Saif-Yehia-Mosaad/Task-1'

E:\Task-1>git branch -M main

E:\Task-1>git push -u origin main
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote:
remote: Create a pull request for 'main' on GitHub by visiting:
remote:      https://github.com/Saif-Yehia-Mosaad/Task-1/pull/new/main
remote:
To https://github.com/Saif-Yehia-Mosaad/Task-1
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

E:\Task-1>git branch
* main

E:\Task-1>git log --oneline
01c5a6d (HEAD -> main, origin/main, origin/feature2) Add new line to index.html

E:\Task-1>
