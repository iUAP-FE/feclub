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

- 生成ssh key

```
ssh-keygen -t rsa -C "guoyff@yonyou.com"
```
