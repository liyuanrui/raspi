
### 1、下载exagear
```
wget http://downloads.eltechs.com/exagear-desktop-v-1-5/exagear-desktop-rpi2.tar.gz
```

### 2、解压
```
tar zxvf exagear-desktop-rpi2.tar.gz
```

### 3、上传key
```
scp pk-000000004587.key  pi@192.168.9.62:/home/pi/exagear
```

### 4、安装
```
sudo ./install-exagear.sh
```

### 5、安装locales软件包
```
apt-get install locales
```

### 6、配置locales软件包
```
dpkg-reconfigure locales
在界面中钩选上“zh_CN.UTF-8”即可
系统默认的区域默认None即可
```

### 7、设置中文区域
```
export LC_ALL=zh_CN.UTF-8
```

### 8、安装中文字体和输入法
```
apt-get install ttf-wqy-zenhei
apt-get install scim-pinyin
```