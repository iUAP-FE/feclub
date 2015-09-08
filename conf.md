# 基本环境搭建

## Node（以windows为例）

- 下载[nodejs](https://nodejs.org/)并安装
- 配置环境变量

```
PATH = C:\Program Files\nodejs;
```

- 在nodejs的安装目录下新增node_global和node_cache目录，并使用npm配置：

```
npm config set prefix "C:\Program Files\nodejs\node_global" 
npm config set cache "C:\Program Files\nodejs\node_cache"
```

- 再次配置环境变量

```
PATH = C:\Program Files\nodejs\node_global;
NODE_PATH = C:\Program Files\nodejs\node_global\node_modules;
```


## Git（以windows为例）

- 下载Git
- 配置环境变量
- 客户端基本配置
- 设置Git的user name和email

``` 
git config --global user.name "GuoYongfeng"
git config --global user.email "guoyff@yonyou.com"
```

- 简单别名配置

```
git config --global alias.st status
git config --global alias.co checkout
git config --global alias.ci commit
git config --global alias.br branch
....

```

- 生成ssh key

```
ssh-keygen -t rsa -C "guoyff@yonyou.com"
```

## 打通github和git

- 开通github账号，方便技术交流和信息获取
- 获取本地的public key

```
cat ~/ssh/id_rsa.pub
```

- 将获得的public key添加在github账户上：

> 右上角点击头像-> 点击settings-> 点击SSH KEYS-> 点击ADD SSH KEYS-> 将获取的public key粘贴于此

- 在github上新建一个仓库

- 在本地新建一个练习目录

```
# 创建一个目录
mkdir test
# 进入所创建的目录
cd test
# 初始化一个git仓库
git init
# 为这个仓库添加一个远程地址
git remote add origin ***
# 新建两个测试文件
touch .gitignore README.md
# 把文件添加到暂存区
git add --all
# 把文件添加到本地版本库
git commit -m "comments"
# 将本地版本库的资源推送到远程服务器
git push -u origin master
```
