# 第1节：GitBook命令

当然，build 命令可以指定路径：

```shell
gitbook build [书籍路径] [输出路径]
```

如果要指定目录,那么添加在init后面

```
gitbook init ./directory
```

serve 命令也可以指定端口：

```shell
gitbook serve --port 2333
```



其它常用的命令:

gitbook init //初始化目录文件
gitbook help //列出gitbook所有的命令
gitbook --help //输出gitbook-cli的帮助信息
gitbook build //生成静态网页
gitbook serve //生成静态网页并运行服务器
gitbook build --gitbook=2.0.1 //生成时指定gitbook的版本, 本地没有会先下载
gitbook ls //列出本地所有的gitbook版本
gitbook ls-remote //列出远程可用的gitbook版本
gitbook fetch 标签/版本号 //安装对应的gitbook版本
gitbook update //更新到gitbook的最新版本
gitbook uninstall 2.0.1 //卸载对应的gitbook版本
gitbook build --log=debug //指定log的级别

gitbook builid --debug //输出错误信息
--------------------- 