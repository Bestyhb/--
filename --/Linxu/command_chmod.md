## chmod (change mode)
文字设定法
数字设定法
八进制数指定权限，文件或目录的权限是由9个权限位进行控制，每3位为1组。分别是User、Group、Other。
user - 文件所有者的读、写、执行
group - 用户组的读、写、执行
other - 其他用户的读、写、执行
Linux/Unix文件权限分为三级：文件所有者(Owner)、用户组(group)、其他用户（Other Users）
![chmod](https://www.runoob.com/wp-content/uploads/2014/08/file-permissions-rwx.jpg)
只有owner和root用户能够修改文件、目录的权限