## TortoiseGit生成.PPK拓展名的密钥

TortoiseGit 使用扩展名为ppk的密钥，而不是ssh-keygen生成的rsa密钥。使用命令ssh-keygen -C "邮箱地址" -t rsa产生的密钥在TortoiseGit中不能用。而基于git的开发必须要用到rsa密钥，因此需要用到TortoiseGit的putty key generator工具来生成既适用于git的rsa密钥也适用于TortoiseGit的ppk密钥，具体配置步骤如下：

    1.运行TortoiseGit开始菜单中的puttygen程序，如下图示
![](https://i.imgur.com/fnZORuh.png)

    2.Import key

~/.ssh > 选取文件id_rsa

    3.Save private key

![](https://i.imgur.com/KIbpEcU.png)

    4.Settings > Git> Remote

![](https://i.imgur.com/rZLnZMn.png)