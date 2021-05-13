# git 的使用方法

1. git 如何安装，如何查看git是否安装成功

   去git官网下载安装，然后在cmd 打开执行 git --version

2. 用户和邮箱配置

   git config --global user.name ""

   git config --global user.email ""

3. 如何上传代码到自己的仓库

   git status     //git 仓库状态

   git add xx    //文件添加到暂存区

   git  commit  -m  "备注" //提交代码

4. 如何查看自己提交的历史记录

   git log --author=huhuan

5. git 删除文件

   右键删除或者 git rm xx 

6. 文件重命名

   git mv 改动前名字 改动后名字

7. 查看文件的历史变化

   git log -p home/demo.html

8. 操作失误回到上次提交状态

   git checkout -- XX 

9. 查看不同

   git --diff

10. 撤销追踪，从暂存区撤销

    git  reset HEAD

11. 回到指定的版本

    git reset  --hard HEAD^

    git reset --hard ID(版本ID)

12.指定的文件回到指定的版本 ID

​		git checkout ID -- xx

13. 将代码推送到远程仓库

     git push origin master

14.给版本添加标签，管理各个版本

​		git tag  v1.0   //默认添加最新的版本上

​		git tag v1.5  ID //指定版本给标签

​		git tag -d v0.5   //删除标签

​		git push origin v1.0  //将标签推送到远程仓库

15. 创建分支，多人协作开发

    git branch XXX  //创建分支

    git checkout xxx //切换分支

    git branch //查看分支

    git branch -d xxx  //删除分支 -D强制删除

    git checkout -b xxx //创建分支并切换到当前分支

16. 合并分支代码

    切换到主分支之后 git merge xxx

17. 合并分支冲突

    git merge -abort 忽略其他分支代码，保留当前的分支的代码

    手动修改，修改完成后 git commit 添加冲突备注，然后esc 退出 ：wq!  
    
18. 查看版本路线

    git log --oneline --graph

19. 删除分支

    git push origin --delete xx 

20. 处理冲突

    git merge xx  然后"i" 修改然后wq!;

21. 不同人修改了相同的代码

    git config --add --local user.name ‘xx'

    git config --add --local user.emaill ‘xx'

    git branch -av   //查看分支 

    git fetch  //获取远程分支

    git checkout -b xx remotes /xx/xx //创建本地分支并和远程分支产生关联

22. 谷歌浏览器的github 的工具

    octotree 

    enhanced github

    gitzip for github







