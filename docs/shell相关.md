# 查看当前使用的 shell 类型

一个并非所有`shell`都支持的方式:

```shell
echo $0
```

只能查看系统默认`shell`类型，不能查看当前`shell`类型:

```shell
echo $SHELL
```

# 查看系统中安装了哪些 shell

```shell
cat /etc/shells
```

# 修改系统默认 shell

可以先通过`cat /etc/shells`查看系统中已安装的`shell`有哪些，然后通过`chsh -s`命令选择默认`shell`

```shell
chsh -s /usr/bin/bash
```
