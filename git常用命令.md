# git常用命令

1. `git init`   创建一个版本库（可在空或非空文件夹创建）
2. `git add "filename"\*` 把工作区中某个文件或者全部文件添加到**暂存区**
3. `git commit -m "description"`  把**暂存区**得内容提交到**当前分支**
4. `git status` 当前仓库的状态
5. `git log [--pretty=oneline]` 显示从最近到最远得提交日志
6. `git reset --hard HEAD^\commit id` 回退到上一个版本或某个版本
7. `git relog` 每一次命令
8. `git diff HEAD -- "filename"`文件在**工作区**和**版本库**的区别
9. `git checkout --"filename"` 丢弃**工作区**对该文件的修改
10. `git reset HEAD "filename"` 可以把**暂存区**的修改撤销，重新放回**工作区**
11. `git rm "filename" + git commit -m "description"`在**版本库**中删除文件
12. `git remote add arigin "your git repository"`  把远程库和本地库关联，远程库名origin
13. `git push [-u]  origin master` 把本地库的内容推送到远程，当远程库为空时加**-u**
14. `git clone "your git repository"` clone 远程的库到本地
15. `git checkout -b dev`创建dev仓库并切换到dev仓库
16. `git branch dev`创建dev分支
17. `git checkout dev`切换到dev分支
18. `git branch` 查看当前分支
19. `git merge dev`把dev合并到当前分支（默认fast forward模式合并）
20. `git branch -d dev`删除dev分支
21. `git log --graph` 命令可以看到分支合并图
22. `git  merge --no-ff -m "merge with no-ff" dev` 不以**fast forward**模式合并分支（方便查看merge记录）
23. `git stash` 把当前工作现场存储起来
24. `git stash list` 查看存储的**工作现场**
25. `git stash apply/git stash pop` 恢复现场，pop表示恢复时删除stash内的内容
26. `git branch -D  dev`强制删除dev分支
27. `git checkout -b dev origin/dev`创建远程的dev分支到本地
28. `git pull`从远程库抓取最新的提交
29. `git branch --set-upstream-to <branch-name> origin/<branch-name>`把本地分子和远程分支关联
30. `git tag "name"` 给当前分支中的commit打上标签
31. `git show "tagname"`查看该标签的信息 
32. `git tag`查看所有标签
33. `git push origin "tagname"` 推送一个本地标签
34. `git push origin --tags`推送所有未推送过的标签
35. `git tag -d "tagname"`删除一个本地标签
36. `git push origin :refs/tags/<tagname>`删除一个远程标签

# over

![工作区暂存区和版本库](https://cdn.liaoxuefeng.com/cdn/files/attachments/001384907702917346729e9afbf4127b6dfbae9207af016000/0)

![分支信息](https://cdn.liaoxuefeng.com/cdn/files/attachments/0013849087937492135fbf4bbd24dfcbc18349a8a59d36d000/0)

![分支信息](https://cdn.liaoxuefeng.com/cdn/files/attachments/0013849088235627813efe7649b4f008900e5365bb72323000/0)

![](https://cdn.liaoxuefeng.com/cdn/files/attachments/00138490883510324231a837e5d4aee844d3e4692ba50f5000/0)

> 以上内容全部是根据廖雪峰的git教程总结  **[官方网址](https://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000)**

