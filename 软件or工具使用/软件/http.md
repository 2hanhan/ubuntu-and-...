
## 下载安装windows版本
这个玩意有界面
https://github.com/Fndroid/clash_for_windows_pkg/releases/tag/0.20.6
解压x64 linux版本
```bash
./cfw
```
## 设置系统代理
在系统设置网络中，设置网络代理手动如下5行
- 127.0.0.1 7890
- 127.0.0.1 7890
-
- 127.0.0.1 7891
- localhost, 127.0.0.0/8, ::1
然后不用的时候设置为自动就行

## 添加配置文件
路径如下ctrl + h 查看隐藏
`.config/clash`
添加`config.yaml`

## git 设置代理
```bash
git config --global http.proxy 'http://127.0.0.1:7890'
```

# apt临时代理
```
sudo apt-get -o Acquire::http::proxy="http://127.0.0.1:7890/" update
```
