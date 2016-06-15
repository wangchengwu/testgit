

#Git SSH Key 生成步骤

Git是分布式的代码管理工具，远程的代码管理是基于SSH的，所以要使用远程的Git则需要SSH的配置。

####一 、设置Git的user name和email：

$ git config --global user.name "xuhaiyan"

$ git config --global user.email "haiyan.xu.vip@gmail.com"


####二、生成SSH密钥过程：
1.查看是否已经有了ssh密钥：cd ~/.ssh
如果没有密钥则不会有此文件夹，有则备份删除
2.生存密钥：

    $ ssh-keygen -t rsa -C “haiyan.xu.vip@gmail.com”
    按3个回车，密码为空。


    Your identification has been saved in /home/tekkub/.ssh/id_rsa.
    Your public key has been saved in /home/tekkub/.ssh/id_rsa.pub.
    The key fingerprint is:
    ………………

最后得到了两个文件：id_rsa和id_rsa.pub

##Git修改提交的用户名和Email
$ git commit --amend --author='Your Name <you@example.com>'
















#####删除文件夹下的所有 .git 文件

    find . -name ".git" | xargs rm -Rf

