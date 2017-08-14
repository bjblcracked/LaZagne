
__The LaZagne Project !!!__
==

Description



github地址：https://github.com/AlessandroZ/LaZagne 2000+的点赞量。

用途太多了：

趁着心仪的妹子不注意，插上u盘，跑一下程序。浏览器上存储的所有密码，就都得到了。什么邮箱密码啊、游戏密码啊，想怎么看就怎么看。
企业办公室入侵，取的法律授权，直接进入被控制的企业，对部分员工电脑执行该程序，获得非常重要的各类信息，如web系统的账号、svn/git账号密码等。
使用方法： 支持linux、mac、windows不同操作系统，因为不同操作系统密码存储形式不一样，所以作者构建了不同的项目。

python源码，直接执行即可。
windows的话，可以下载exe执行。
源码写的很牛逼，对于进阶python的，可以读一下作者写的源码。






----
The __LaZagne project__ is an open source application used to __retrieve lots of passwords__ stored on a local computer. 
Each software stores its passwords using different techniques (plaintext, APIs, custom algorithms, databases, etc.). This tool has been developed for the purpose of finding these passwords for the most commonly-used software. 

<p align="center"><img src="./pictures/lazagne.png" alt="The LaZagne project"></p>

This project has been added to [pupy](https://github.com/n1nj4sec/pupy/) as a post-exploitation module. Python code will be interpreted in memory without touching the disk and it works on Windows and Linux host. The last Linux release is not up to date so I recommend to use pupy to use it. 

Standalones
----
Standalones are now available here: https://github.com/AlessandroZ/LaZagne/releases/

Usage
----
* Retrieve version
```
laZagne.exe --version
```

* Launch all modules
```
laZagne.exe all
```

* Launch only a specific module
```
laZagne.exe browsers
```

* Launch only a specific software script
```
laZagne.exe browsers -f (for firefox)
```

* Write all passwords found into a file (-oN for Normal txt, -oJ for Json, -oA for All)
```
laZagne.exe all -oN
```

* Get help
```
laZagne.exe -h
laZagne.exe browsers -h
```

* Use a file for dictionary attacks (used only when it's necessary: mozilla masterpassword, system hahes, etc.). The file has to be a wordlist in cleartext (no rainbow), it has not been optmized to be fast but could useful for basic passwords.
```
laZagne.exe all -path file.txt
```

* Change verbosity mode (2 different levels)
```
laZagne.exe all -vv
```

__Note: For wifi passwords \ Windows Secrets, launch it with administrator privileges (UAC Authentication / sudo)__

Supported software
----

<p align="center"><img src="./pictures/softwares.png" alt="The LaZagne project"></p>

(*) used by many tools to store passwords: Chrome, Owncloud, Evolution, KMail, etc.

For developers
----
Please refer to the wiki before opening an issue to understand how to compile the project or to develop a new module.
https://github.com/AlessandroZ/LaZagne/wiki


Special thanks
----
* Harmjoy for [KeeThief](https://github.com/HarmJ0y/KeeThief/)
* n1nj4sec for his [mimipy](https://github.com/n1nj4sec/mimipy) module
* Benjamin DELPY for [mimikatz](https://github.com/gentilkiwi/mimikatz), which helps me to understand some Windows API.
* [Creddump](https://github.com/moyix/creddump)
* All [contributors](https://github.com/AlessandroZ/LaZagne/graphs/contributors) who help me on this project

----
| __Alessandro ZANNI__    |
| ------------- |
| __zanni.alessandro@gmail.com__  |

