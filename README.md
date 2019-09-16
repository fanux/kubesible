# kubesible
利用kubernetes对宿主机进行运维

sibelet 类似 kubelet但是它的作用不是去起pod，而是监听CRD在宿主机上干些运维工作。

如 同步时间，配置/etc/hosts 安装一些东西等， 或者是帮助我们检查机器的期望状态与实际状态是否符合

比如监控机器的磁盘大小，如果超过85%就对/var/log/messages进行清理，或者对docker镜像进行清理等。

凡事需要对宿主机进行一些自动化操作的事情都可以通过kubesible进行。
