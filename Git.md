  **2018年5月9号**  
  
 大三下半学期，现已进入实训阶段第二周，为了完成一款在线支付项目，再次复习Git，以及github的一些操作。（现在脑子真的记不住东西了，能把自己给气死的那种）   
## Git  
其实完成这个项目所需要的git操作指令并不多，详情如下:  
1.git init 在当前的所处的目录下创建本地git仓库  
2.git add . 或者是 git add <文件名称> 将指定文件添加到暂存区  
3.git commit -m "<提交描述>" 提交暂存区到仓库区  
4.git remote add origin [url] 添加一个远程仓库  
5.git config --global core.autocrlf false/true git有自动转换的功能，禁止或开启自动转换（错误提示为warning:LF will be replaced by CRLF.. 原因:在Windows中换行符为CRLF，Linux中是LF，git开启自动转换默认为LF）  
6.git push origin master 将本地指定分支上传到远程仓库（执行该命令语句是会让你输入github的登录名和密码）  
7.git clone [url] 下载一个项目和它整个代码历史  
8.git pull origin master 将远程仓库取回与本地仓库合并  
9.git pull origin master --allow-unrelated-histories （不明其理，意思是允许合并不相关的历史之类的 当 git pull失败并提示fatal: refusing to merge unrelated histories时可用）  
10.git status 显示变更文件  
11.git log 显示当前分支的版本历史，其中HEAD->mastr表示的是本地当前版本历史，origin/master是远程仓库的版本历史  
[其它Git指令](http://www.ruanyifeng.com/blog/2015/12/git-cheat-sheet.html)  
目前需要的指令并不多还有一些bash指令可能会用到:  
rm -rf .git 删除本地仓库  .git是一个隐藏文件夹当创建本地仓库时会创建，r该目录下的所有子文件，f强制删除  
clear 清除git bash界面的命令与响应  
cd <文件夹名> 移动到指定目录  
