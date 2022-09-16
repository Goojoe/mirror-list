## 1.软件下载镜像

- [淘宝](https://registry.npmmirror.com/binary.html?path=git-for-windows/)

- [清华大学](https://mirrors.tuna.tsinghua.edu.cn/github-release/git-for-windows/git/LatestRelease/)

## 2.代理设置

终端输入

```
# http代理
git config --global http.https://github.com.proxy http://127.0.0.1:7890
# https代理
git config --global https.https://github.com.proxy http://127.0.0.1:7890
```

配置保存在`~/.gitconfig`

## 3.Clone镜像

```
# 设置为Gitclone.com
git config --global url."https://gitclone.com/".insteadOf https://
```



## 其他

### 设置用户名邮箱

```
git config --global user.name "username"
git config --global user.email "email@email.com"
```

## 设置ssh

```
mkdir ~/.ssh
cd ~/.ssh
ssh-keygen -t rsa -b 4096 -C "email@email.com"
# 回车3次
# 前往https://github.com/settings/keys添加id_rsa.pub内容里的公钥
# 测试连接
ssh -T git@github.com
```

## GPG配置
[github GPG 配置](https://segmentfault.com/a/1190000016330472)