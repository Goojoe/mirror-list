## 1.软件下载镜像

前往[VSCode官网下载页](https://code.visualstudio.com/Download)

### 获取下载链接

1.点击下载进入下载页复制链接

2.使用curl

前往[VScode全部版本](https://code.visualstudio.com/docs/supporting/faq#_previous-release-versions)

选择好系统对应系统包后将`{version}`改为`latest`(最新版),使用curl获取链接

```
curl https://update.code.visualstudio.com/latest/win32-x64-archive/stable

Found. Redirecting to https://az764295.vo.msecnd.net/stable/74b1f979648cc44d385a2286793c226e611f59e7/VSCode-win32-x64-1.71.2.zip
```

### 加速方法

将下载链接里的`az764295.vo.msecnd.net`(可能不同)修改为`vscode.cdn.azure.cn`

例子

```
https://vscode.cdn.azure.cn/stable/74b1f979648cc44d385a2286793c226e611f59e7/VSCode-win32-x64-1.71.2.zip
```

## 2.VSCode代理

`Ctrl`+`,`打开设置搜索`proxy`

修改http:Proxy

```
# http
http://127.0.0.1:7890
# socks5
socks5://127.0.0.1:7890
```

修改Http: Proxy Support为

`override`

>为扩展启用代理支持，覆盖请求选项

