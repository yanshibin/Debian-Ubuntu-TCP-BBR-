# 下载地址
```
wget --no-check-certificate -qO 'BBR.sh' 'https://raw.githubusercontent.com/yanshibin/Debian-Ubuntu-TCP-BBR-/master/BBR.sh' && chmod a+x BBR.sh
```
## 使用方法:
普通模式,最后需要按下回车才会重启.

```
bash BBR.sh
```
强制模式,全自动(如果中间不报错),不需要按下回车.

```
bash BBR.sh -f
```
指定安装内核版本,以4.11.9为例.

```
bash BBR.sh -f v4.11.9
```
### 检测:
重启后运行以下命令,结果不为空,则开启BBR成功.
```
lsmod |grep 'bbr'
```
