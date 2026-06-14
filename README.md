furkanses@DESKTOP:/c/Users/Furkan/Desktop/git-github-demo$ echo "main icerik 1" > a.txt
furkanses@DESKTOP:/c/Users/Furkan/Desktop/git-github-demo$ git add .
furkanses@DESKTOP:/c/Users/Furkan/Desktop/git-github-demo$ git commit -m "main yeni commit"
[main 7dc0394] main yeni commit
 1 file changed, 1 insertion(+), 1 deletion(-)
furkanses@DESKTOP:/c/Users/Furkan/Desktop/git-github-demo$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Writing objects: 100% (3/3), 238 bytes | 26.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To github.com:furkanses/git-github-demo.git
   c9c8ea9..7dc0394  main -> main
furkanses@DESKTOP:/c/Users/Furkan/Desktop/git-github-demo$ git checkout child
Switched to branch 'child'
furkanses@DESKTOP:/c/Users/Furkan/Desktop/git-github-demo$ echo "child icerik 2" > a.txt
furkanses@DESKTOP:/c/Users/Furkan/Desktop/git-github-demo$ git add .
furkanses@DESKTOP:/c/Users/Furkan/Desktop/git-github-demo$ git commit -m "child yeni commit"
[child 7151806] child yeni commit
 1 file changed, 1 insertion(+), 1 deletion(-)
furkanses@DESKTOP:/c/Users/Furkan/Desktop/git-github-demo$ git push
fatal: The current branch child has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin child

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

furkanses@DESKTOP:/c/Users/Furkan/Desktop/git-github-demo$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
furkanses@DESKTOP:/c/Users/Furkan/Desktop/git-github-demo$ git merge child
Auto-merging a.txt
CONFLICT (content): Merge conflict in a.txt
Automatic merge failed; fix conflicts and then commit the result.
furkanses@DESKTOP:/c/Users/Furkan/Desktop/git-github-demo$ cat a.txt
<<<<<<< HEAD
main icerik 1
=======
child icerik 2
>>>>>>> child
furkanses@DESKTOP:/c/Users/Furkan/Desktop/git-github-demo$ echo "main icerik 1" > a.txt
furkanses@DESKTOP:/c/Users/Furkan/Desktop/git-github-demo$ git add .
furkanses@DESKTOP:/c/Users/Furkan/Desktop/git-github-demo$ git commit -m "çakışma çözüldü"
[main f8d0169] çakışma çözüldü
furkanses@DESKTOP:/c/Users/Furkan/Desktop/git-github-demo$ git push
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 16 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (4/4), 424 bytes | 35.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
To github.com:furkanses/git-github-demo.git
   7dc0394..f8d0169  main -> main

ÖNEMLİ  ==>   DERSTE YAPTIĞIM DEMO REPOSUNU SİLDİĞİM İÇİN TEKRAR AYNISINI YAPTIM
