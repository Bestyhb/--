//
本文档仅包含课堂讲义内容，扩展部分根据主题列为每份的单独文档。
//
# 第一章 Linux、H5场景制作、Mockplus交互设计
## 1.1Linux初识
## 1.2 Linux基础、核心命令（上）
## 1.3 Linux核心命令（下）
## 14 Linux服务器搭建、项目部署
**Linux/Unix压缩文件及其工具**

默认支持以下三种压缩文件格式：
bzip2(.bz2)
压缩文件，但不能压缩目录，压缩后源文件消失。
gzip(.gz)
用于压缩文件，不能用于目录的压缩，压缩后源文件消失。
zip(.zip)
用于文件和目录的压缩，压缩后源文件存在。


**tar(.tar)**
| v | 列出所操作的和结果文件 |
| f | file | 文件参数 |
| c | 打包 |
| x | 解包 |
| r | 追加文件至文档  |
| t | 列出文档内容    |
| u | 更新文档中的文件|
| z | gzip           |
| j | bzip2          |
> 常用的 tar 命令中必须添加 "f" 参数，以承接文件，一般作为最后一个必备的参数。所以常用的tar命令格式一般为` # tar -***t [file]`
`tar -cf tarname.filetype.tar filename.filetype` 打包
`tar -xf tarname.tar` 解包
`tar -v` 显示打包信息
`tar -f` 包内容为文件
`tar -z` 同时使用gzip进行压缩和解压
`tar -j` 同时使用bzip2进行压缩和解压
`tar -zcf tarfilename.filetype.tar files.file` gzip压缩
`tar -zxf tarfilename.filetype.tar files.file` gzip解压
`tar -cf alljpg.tar *.jpg`
`tar -cf allmd.tar *.md`
`tar -cf alltxt.tar *.txt`
`tar -cf alltar.tar *.tar`

**bzip2(Bzip COmpressed Archive):**  
`bzip2 -z filename.file` 压缩单个文件
`bzip2 filename.file` 压缩单个文件
`bzip2 file1 file2` 压缩多个文件
`bzip2 -d file.bz2` 解压一个文件
`bzip2 -d file1.bz2 file2.bz2` 解压多个文件

**gzip:**  
> gzip比bzip压缩率更大。
`gzip file.file`
`gzip file1.file file2.file`
`gzip -d file1.gz`
`gzip -d file1.gz file2.gz`

zip:  
> Linux不推荐使用zip进行通常的压缩操作。
`zip zipname.zip file1.file file2.file` 压缩一个及多个文件
`zip -r zipname.zip dirname` 压缩目录
`uzip zipname.zip`

打包和压缩的不同
打包：为了方便归档、管理，可以将一个文件夹huo多个零散文件，变为一个独立文件
压缩：为了减少磁盘空间的消耗


操作系统的分类：家用系统和服务器系统
服务器只是内部的硬件结构不同、安装的运行环境不同。如果服务器需要部署到互联网就需要安装服务器程序，否则还是一台普通用途的电脑。
一台电脑进入互联网需要得到一个具体的IP地址，由网络服务商提供。

域名解析、浏览器请求domain（IP） → 指定IP的服务器，会找固定的网络线路进行联接。
.com
.org
.net
.cn
.kr
.jp
中国2019年，建立中国主根服务器1台，辅根服务器3台。
浏览器输入网址 → DNS域名服务器查询IP地址 → 链接指定IP电脑
服务器软件：
APACH： PHP
TOMCAT： JAVA
IIS： C#, .net

网络安装Apache、MySQL
Ubuntu：`# apt install apache2`
CentOS：`# yum install httpd`

## H5场景基础
## H5表单控件、组件（上）
## Mockplus基础组件、控件-表格
## Mockplus布局、交互、综合布局

# 第二章 Markdown轻文档制作
## Markdown-1
## Markdown-2

# 第三章 Office办公工具
## Office-1
## Office-2
## Office-3
## Office-4

# 第四章 XMind思维导图
## XMind-1
## XMind-2

# 第五章 H5+CSS3
## H5+CSS3-1
## H5+CSS3-2
## H5+CSS3-3
## H5+CSS3-4
## H5+CSS3-5
## H5+CSS3-6

#第六章 Python核心语法
##Python核心语法-1
##Python核心语法-2
##Python核心语法-3
##Python核心语法-4
##Python核心语法-5
##Python核心语法-6