# Git使用
1、启动Git Bash命令行，输入 git clone https://github.com/zhiyishangcheng/mall.git <br/>
2、clone执行成功以后打开文件夹，输入 cd mall <br/>
3、在项目文件夹可以进行的操作：<br/>
  （1）新建文件夹：mkdir dirname <br/>
  （2）新建文件：touch a.html b.css c.js【可以新建一个，也可以新建多个】 <br/>
4、git add . <br/>
5、git commit -m "changes log" <br/>
6、git push -u origin master ->输入账号->输入密码
# git pull常见操作
1、取回origin主机的next分支，与本地的master分支合并，需要写成下面这样。<br/>
$ git pull origin next:master<br/>
2、如果省略本地分支名，则表示远程分支是与当前分支合并。<br/>
$ git pull origin next（该命令表示：取回origin/next分支，再与当前分支合并）<br/>
3、如果当前分支与远程分支存在追踪关系，git pull就可以省略远程分支名。<br/>
$ git pull origin（该命令表示：本地的当前分支自动与对应的origin主机”追踪分支”(remote-tracking branch)进行合并）<br/>
4、如果当前分支只有一个追踪分支，连远程主机名都可以省略。<br/>
$ git pull（该命令表示：当前分支自动与唯一一个追踪分支进行合并）
