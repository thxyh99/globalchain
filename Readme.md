[Readme](https://docs.google.com/document/d/1sFWk95Ap3gjQcRFr3kq4hvU1SFk0EtGCIeW2IKJAVD0/edit#)
# Git 初体验 #

1、对 Git 进行初始化：

    git init

2、将项目所有文件纳入到 Git 中：

    git add -A

3、检查 Git 状态：

    git status

4、保留改动并提交：

    git commit -m “Initial commit”

5、查看历史提交记录：

    git log

6、恢复被删除文件：

    git checkout -f

7、创建新的分支：

    git checkout -b branch

8、合并分支：

    git merge branch

9、删除分支：

    git branch -d branch

10、对Git 进行用户名和邮箱进行设置：

    git config --global user.name “thxyh99”
    git config --global user.email xieyihong@globalegrow.com

11、添加远程代码库提交地址，并提交代码：

    git remote add origin git@github.com:thxyh99/hello.git
    git push -u origin master



# 什么是 GitHub？ #
1、 注册 GitHub 账号

2、 为 GitHub 账号设置 SSH Key

    eval “$(ssh-agent -s)”
    ssh-add ~/.ssh/id_rsa
    cat ~/.ssh/id_rsa.pub

3、 提交代码到 Github

    git remote add origin git@github.com:thxyh99/hello.git
    git push -u origin master


# 前言 #

**PHP**

PHP 全称是 PHP: Hypertext Preprocessor，译为：『超文本预处理器』。是一门开源服务器脚本语言。PHP 市场占有率最高的服务器端脚本语言，Alexa 世界排名前一千万 的网站中有 82.6% 使用 PHP 构建。

**MVC**

MVC 是三个单词的首字母缩写，它们是 Model（模型）、View（视图）和 Controller（控制器），是一种软件架构设计模式。

最上面的一层，是直接面向最终用户的『视图层』（View）。它是提供给用户的操作界面，是程序的外壳。
最底下的一层，是核心的『数据层』（Model），也就是程序需要操作的数据或信息。
中间的一层，就是『控制层』（Controller），它负责根据用户从『视图层』输入的指令，选取『数据层』中的数据，然后对其进行相应的操作，产生最终结果。

# 环境部署 #
 
**Atom**

Atom 是由 GitHub 官方在 2014 年 2 月推出的一款开源的跨平台代码编辑器，由于 Atom 的界面优雅、易上手、插件丰富等优点，使得其在发布后受到圈内不少程序员的追捧和赞赏。

**Sublime Text**
Sublime Text 也是一款跨平台代码编辑器，是非常棒的 Atom 替代品。

**命令行**

命令行是程序员的好伙伴，如果你立志成为一名优秀的程序员，熟练的命令行操作也是必不可少的。命令行客户端 Mac 下我们使用 iTerm2，Windows 下使用 GitHub 出品的 Git for Windows。

**VirtualBox**

VirtualBox 号称是最强的免费虚拟机软件，是 Oracle 公司的开源虚拟机软件。本书中我们用来运行 Homestead 虚拟主机。

**Vagrant**

Vagrant 是用来管理虚拟机的工具，主要功能是确保项目参与人员各自的机器上都能拥有一致的开发环境。

**Homestead**

Homestead 利用 Vagrantfile 提供的便利，定制了一整套的可配置、可移植和复用的 Laravel 开发环境。Homestead 虚拟机里面包含了 Nginx Web 服务器、PHP 7.0、MySQL、Postgres、Redis、Memcached、Node，以及所有你在使用 Laravel 开发时需要用到的各种软件。

**Homestead 管理脚本**

Homestead 脚本使用 Ruby 和 Shell 脚本编写而成。原理是对 Vagrantfile 文件做定制。将从 `~/Homestead/Homestead.yaml` 读取的配置信息，在 provision 时，解析为 Vagrant 命令并进行对虚拟机的配置。Homestead 脚本的作用在于，提供了极其简单易用的接口，使我们只需要通过傻瓜化配置，即可完成复杂的任务。

**Composer**

Composer 是一款跨平台的 PHP 依赖管理工具，其创作灵感来源于 `Node.js` 的 NPM 与 Ruby 的 Bundler。Laravel 使用 Composer 来作为扩展包的管理工具，默认的扩展包依赖在 `composer.json` 文件里。你可以利用 Composer 结合 其它开源扩展包 来达到快速建站的目的。

**Git**

Git 是 Linux 的创始人 Linus Torvalds 开源的一款分布式版本控制系统，在现代化的项目开发中，Git 基本上是标配。

**GitHub**

GitHub 是目前全球最大的代码托管平台，许多非常著名的项目如 Linux、PHP、Swift、Laravel 等都托管在 GitHub 上。

**Heroku**

Heroku 是一个支持多种编程语言的 PaaS (Platform-as-a-Service)。本书中我们使用 Heroku 来模拟部署上线代码。

**Git 分支**

Git 允许你把工作从开发主线上分离开来，以免影响开发主线。 Git 主分支的名字，默认叫做Master。它是自动建立的，版本库初始化以后，默认就是在主分支在进行开发。

**SSH**

SSH 为 Secure Shell 的缩写，SSH 为建立在应用层基础上的安全协议。SSH 是目前较可靠，专为远程登录会话和其他网络服务提供安全性的协议。在此课程中，我们使用 SSH 免密码登录 Homestead 虚拟机、免密码 Push 代码到 GitHub、免密码部署代码到 Heroku。

# 构建页面和优化页面 #
 
**Artisan**

Artisan 是 Laravel 提供的 CLI（命令行接口），它提供了非常多实用的命令来帮助我们开发 Laravel 应用。

**Bootstrap**

在本书的教学过程中我们使用 Bootstrap 来作为演示应用的前端 UI 框架。

**NPM**

NPM 是 `Node.js`（一个基于 Google V8 引擎的 JavaScript 运行环境）的包管理和分发工具。Composer 的一些概念也是从 NPM 中借鉴过来的，因此 NPM 也有个类似 `composer.json` 文件的 `package.json` 文件，Laravel 默认会为每个新建的项目自动生成该文件。

**Yarn**

由于 NPM 的安装速度，安全性和稳定性等都饱受开发者的诟病，本书使用 Facebook 在 2016 年的 10 月份开源的 Yarn 来作为 NPM 的替代品。Yarn 最大的特点是安装依赖速度快，还有支持本地缓存。

**SASS**

Sass 是一种可用于编写 CSS 的语言，是现代化的 CSS 编写方式，借助 Sass 我们可以少写很多 CSS 代码，并使样式代码的编写更加灵活多变。

**Laravel Mix**

Laravel Mix 一款前端任务自动化管理工具，使用了工作流的模式对制定好的任务依次执行。Mix 提供了简洁流畅的 API，让你能够为你的 Laravel 应用定义 Webpack 编译任务。

**Blade**

Blade 是 Laravel 所提供的一个简单且强大的模板引擎。Blade 视图文件使用 `.blade.php` 做为扩展名，通常保存于 `resources/views` 文件夹内。

**路由**

特指 Laravel 的路由配置信息，存放在 `routes/web.php` 中，使用 Route 类方法来配置 HTTP 请求对应处理的控制器。