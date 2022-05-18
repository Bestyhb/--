**alias**
若仅使用`alias`命令进行别名设置，则重启系统后不会再次生效。
若需要alias设置持续有效，则需要配置相关文件。
有两个文件可以进行配置：

.bashrc
.alias
（.bashrc是系统包含的，.alias是需要创建的。）


source:
1. [bianchen](http://c.biancheng.net/linux/alias.html)
**login(1):** 
mail(1), passwd(1), sh(1), su(1), login.defs(5), nologin(5), passwd(5), securetty(5), getty(8)
**login.def(5):** 
login(1), passwd(1), su(1), passwd(5), shadow(5), pam(8)

**useradd(8):** 
chfn(1), chsh(1), passwd(1), crypt(3), groupadd(8), groupdel(8), groupmod(8), login.defs(5), newusers(8), subgit(5), subuid(5), userdel(8), usermode(8)
**userdel(8):** 
chfn(1), chsh(1), passwd(1), login.def(5), gpasswd(8), groupadd(8), groupdel(8), groupmod(8), subgid(5), subuid(5), useradd(8), usermod(8) 
**usermod(8):** 
chfn(1), chsh(1), passwd(1), crypt(3)(NEEDINSTALL), gpasswd(8), groupadd(8), groupdel(8), groupmod(8), login.defs(5), subgid(5), subuid(5), useradd(8), userdel(8)
**chsh(1):** 
chfn(1), login.defs(5), passwd(5)
**chfn(1):** 
chsh(1), login.defs(5), passwd(5)
**passwd(1):** 
chpasswd(8), passwd(5), shadow(5)
**gpasswd(1):** 
newgrp(1), groupadd(8), groupadd(8), groupmod(8), grpck(8), group(5), gshadow(5)
**groupadd(8):** 
chfn(1), chsh(1), passwd(1), gpasswd(8), groupdel(8), groupmod(8), login.defs(5), useradd(8), userdel(8), usermod(8)
**groupdel(8):** 
chfn(1), chsh(1), passwd(1), gpasswd(8), groupadd(8), groupmod(8), useradd(8), userdel(8), usermod(8)
**groupmod(8):** 
chfn(1), chsh(1), passwd(1), gpasswd(8), groupadd(8), groupdel(8), login.defs(5), useradd(8), userdel(8), usermod(8)

**subgid(5):** 
login.defs(5), newgidmap(1), newuidmap(1), newusers(8), subuid(5), useradd(8), userdel(8), usermod(8), user_namespaces(7)
**subuid(5):** 
login.def(5), newgidmap(1), newuidmap(1), newusers(8), subgid(5), useradd(8), userdel(8), usermod(8), user_namespaces(7)
**shadow(5):** 
chage(1), login(1), passwd(1), passwd(5), pwck(8), pwconv(8), su(1), sulogin(8)
**gshadow(5):**
gpasswd(5), group(5), grpck(8), grpconv(8), newgrp(1)