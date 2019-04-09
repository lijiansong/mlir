## CentOS 6.6 upgrade gcc

```
sudo yum -y install centos-release-scl
sudo yum -y install devtoolset-7-gcc devtoolset-7-gcc-c++ devtoolset-7-binutils
sudo scl enable devtoolset-7 bash
sudo echo "source /opt/rh/devtoolset-7/enable" >>/etc/profile
```

Upgraded gcc will be located in directory `/opt/rh/devtoolset-7/root/usr/bin`, export this path to environment variable：

```
export PATH=/opt/rh/devtoolset-7/root/usr/bin:$PATH
```
