scriptool
=========

some script?


rhel-source.repo
=========
change CDS yum for RHEL6


rpm -qa | grep yum | xargs rpm -e --nodeps

wget http://mirrors.yun-idc.com/centos/6/os/x86_64/Packages/yum-3.2.29-40.el6.centos.noarch.rpm

wget http://mirrors.yun-idc.com/centos/6/os/x86_64/Packages/yum-plugin-fastestmirror-1.1.30-14.el6.noarch.rpm

wget http://mirrors.yun-idc.com/centos/6/os/x86_64/Packages/yum-metadata-parser-1.1.2-16.el6.x86_64.rpm

wget http://mirrors.yun-idc.com/centos/6/os/x86_64/Packages/python-iniparse-0.3.1-2.1.el6.noarch.rpm

rpm -ivh *.rpm

mv /etc/yum.repos.d/rhel-source.repo /etc/yum.repos.d/rhel-source.repo.bak

mv rhel-source.repo /etc/yum.repos.d/rhel-source.repo
