# 2017web-lab01

# 实验目的
1. 学会使用git和github
2. 掌握html5的基本框架
3. 学会利用互联网进行学习

# 实验内容
1. 创建你的第一个网页

# 实验步骤
1. 准备一个USB3.0的U盘
1. 通过百度云下载相关软件，下载地址见对分易的课程资源中的“相关软件下载地址.txt”，将这些软件拷贝到你的U盘。
1. 安装git：双击U盘中的PortableGit-2.14.1-64-bit.7z.exe文件，单击确定按钮解压并安装git到你的U盘。
1. 安装vscode：解压缩U盘中的VSCode-win32-x64-1.16.1.zip到U盘的VSCode-win32-x64-1.16.1目录，双击打开该目录，双击其中的code.exe打开vscode编辑器
1. 单击vscode编辑器的“文件”-“打开文件”菜单，选择解压后的git目录中的etc目录中的bash.bashrc文件，单击“打开”按钮，打开该文件，在该文件最后添加一行内容如下（注意区分字母大小写）：export HOME=/
1. 单击“文件”-“保存”菜单将修改存盘，然后单击“文件”-“退出”关闭vscode编辑器。
1. 通过浏览器访问网址：https://github.com/ ，用你的邮箱注册一个github账号，并通过收到的邮件激活你的github账号
1. 利用你的github账号登录github网站
1. 访问作业链接（我会通过对分易平台发微信消息告诉大家具体的作业链接），然后单击绿色的clone ordownload按钮，可以看到一个类似下面这样的地址：https://github.com/2017webclass1/lab01-your-user-name.git
1. 克隆作业到本地：双击打开U盘中的Git安装目录，在空白处右键创建一个2017fall-web文件夹，双击运行Git安装目录中的git-bash.exe，在出现的命令行窗口中输入命令：

```sh
git config --global user.name "your-user-name"
git config --global user.email your-email
cd 2017fall-web
git clone https://github.com/2017webclass1/lab01-your-user-name.git
ls
cd lab01-your-user-name
git status
```
    
说明：
* git config --global user.name和git config --global user.email 用于配置用户名和邮箱
* cd 命令用于进入指定的文件夹
* git clone 命令用于将网上的代码库复制一份副本到当前文件夹
* git status 命令用于查看代码库的状态
11. 编辑本地作业：用dreamweaver或vscode在2017fall-web文件夹中创建一个index.html文件，添加一些基本的html元素和内容并保存，然后用chrome浏览器打开查看网页效果，如果不满意科通过dreamweaver或vscode继续修改存盘，然后在浏览器中按F5刷新，如此反复，直到满意为止。
12. 提交本地作业：回到git-bash.exe命令行窗口，并输入以下命令：

```sh
git status
git add index.html
git status
git commit -m "create index.html"
git status
```

说明：
* git add index.html 表示添加新创建的或新修改的文件，若新创建或修改了多个文件，则可使用 git add . 命令一次性添加所有新创建或新修改的文件
* git commit -m "description" 表示提交所有修改
13. 将本地作业推送到github网站：

```sh
git push origin master
```
   
14. 在浏览器中访问你的github网站，检查你的作业中是否增加了一个和你U盘中一样的index.html文件。
15. 小结
    今后每次实验的流程基本类似，大致如下：
    1. 访问微信消息中给出的本周作业链接
    1. 克隆作业到本地
    1. 编辑本地作业
    1. 提交本地作业
    1. 将本地作业推送到github网站
    说明：每次对本地作业进行修改后，都要提交本地作业和推送到github网站，确保最新的修改被同步到本地库和网络远程库。
