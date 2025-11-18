# 简介
Git

# 版本选择

本教程使用的版本为Git-2.50.1-64-bit，以下的安装流程皆以此版本为主。

# 安装

 ![[Pasted image 20251118153535.png]]
 首先是Git的相关版本信息，这个直接跳过，选择"Next"。

----
 
![[Pasted image 20251118153844.png]]
下一个界面为Git安装路径，**请根据个人习惯选择安装位置**，我一般喜欢把软件放在D盘。
选择完成后继续点击”Next“进行下一步。

---

![[Pasted image 20251118154248.png]]
这里是Git的安装部件选择，选择你需要的功能。

| 选项                                                               | 解释                                        |
| ---------------------------------------------------------------- | ----------------------------------------- |
| On the Desktop                                                   | 生成桌面图标（一般不选，没人会在桌面上打开Git）                 |
| Open Git Bash here                                               | **必选**，将Git Bash添加到鼠标右键菜单                 |
| Open Git GUI here                                                | **必选**，将Git GUI添加到鼠标右键菜单                  |
| Git LFS                                                          | **必选**，支持大文件（超过Github的100M大小限制）           |
| Associate .git* configuration files with the default text editor | **必选**，将 .git* 配置文件与默认文本编辑器相关联            |
| Associate .sh files to be run with Bash                          | **必选**，关联 .sh （脚本）格式文件                    |
| Check daily for Git for Windows update                           | 检查每日更新，看个人选择                              |
| Add a GIt Bash Profile to Windows Terminal                       | 在WIndows系统命令行增加Git Bash(意思是可以在终端方便的启用Git) |
| Scalar                                                           | 需要管理大规模仓库则选择此选项                           |

---

![[Pasted image 20251118155819.png]]

这个页面表示是否在Windows开始菜单上添加Git启动，如果你觉得方便就添加上，继续”Next“。

---

![[Pasted image 20251118160244.png]]
此处为选择Git的默认编辑器，安装界面给我们提供了很多编辑器以供我们选择。作为网络安全学习的人员，我建议最好使用默认编辑器vim（虽然这个编辑器是纯命令行，操作有些困难）。
>[!note]
>1.注意，若使用**其他编辑器**需要在相应的官网进行下载，同时还要**进行配置**
>2.若选择编辑器为VScode，相关的安装教程会在后面演示（先空着）

---

![[Pasted image 20251118160834.png]]
这个页面是决定初始化新项目(仓库)的主干名字。
* 前一个选项是Git默认，主干为master
* 后一个选项是自定义主干名称，默认为main
随自己心意选择即可，仅仅改变项目主干名。

---

![[Pasted image 20251118161319.png]]
这里是在调整Git的PATH环境变量。
 * 仅从Git Bash使用Git
 * 从命令行以及第三方软件进行Git（**推荐**）
 * 从命令提示符使用 Git 和可选的 Unix 工具（**慎用，这会导致Windows工具被覆盖，除非你是大佬**）

---

![[Pasted image 20251118161953.png]]
此页面表示选择相应的OpenSSH（安全Shell工具的开放源代码版本，Linux 及其他非 Windows 系统的管理员使用此类工具跨平台管理远程系统）。
* 使用Git自带的OpenSSH
* 使用外部OpenSSH
这个普通用户就选择第一个即可，第二个选择的OpenSSH需要自己配置。

---

![[Pasted image 20251118162749.png]]
这个页面是在选择Git的加密库。
* 使用OpenSSL库（强大的加密库，广泛应用于互联网的各个角落，用于保护数据传输的安全）
* 使用Windows安全通道库iH
如果你不是身处需要企业管理证书的组织中使用Git，仅仅是访问GitHub，那么选择第一个。

---

![[Pasted image 20251118163327.png]]
这里是配置Git行尾符号转换。
* 签出 Windows 样式，提交 Unix 样式的行结尾。（**推荐**）
* 按原样签出，提交Unix样式的行结尾。
* 按原样签出，按原样提交。

>[!note]
>GitHub 中公开的代码大部分都是以 Mac 或 Linux 中的 LF（Line Feed）换行。然而，由于 Windows 中是以 CRLF（Carriage Return+ Line Feed）换行的，所以在非对应的编辑器中将不能正常显示。
>使用 Windows 环境的话，请选择推荐的 “Checkout Windows-style，commit Unix-style line endings” 选项。换行符在签出时会自动转换为 CRLF，在提交时则会自动转换为 LF 。


---

![[Pasted image 20251118163816.png]]
为Git Bash配置模拟器终端界面：
* 使用MinTTY（**推荐**）
* 使用cmd
一般来说，MinTTY比cmd好用一些。

---

![[Pasted image 20251118164143.png]]
这里是选择git pull（获取最新的远程仓库分支到本地，并与本地分支合并）的默认行为。
* 默认合并策略（**推荐**）
* 重新基础合并策略（**大佬可以试试**）
* 仅快进合并策略（只是拉取远程分支，合并靠自己）

---

![[Pasted image 20251118164934.png]]
这里是选择一个凭证帮助程序。
* Git 凭证管理（输入账户密码才能登陆远程仓库GitHub）（**必选**）
* 不使用凭证助手

---

![[Pasted image 20251118165322.png]]
这里是配置额外的选项
* 启用文件系统缓存（**推荐，大幅提高性能**）
* 启用符号链接（**该功能的支持需要一些条件**）

点击“Install”就安装完成啦！！！


