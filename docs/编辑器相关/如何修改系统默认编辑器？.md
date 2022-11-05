# 如何修改系统默认编辑器？

在使用`visudo`等命令时，会调用系统默认编辑器，如果此时出现的是`nano`，而我又想用`vim`进行编辑该怎么办呢？

这就需要去修改默认的编辑器了，要用到`update-alternatives`这个命令，通过`--config editor`可以配置编辑器的优先级

```shell
update-alternatives --config editor
```

```
There are 4 choices for the alternative editor (providing /usr/bin/editor).

  Selection    Path                Priority   Status
------------------------------------------------------------
  0            /bin/nano            40        auto mode
  1            /bin/ed             -100       manual mode
  2            /bin/nano            40        manual mode
* 3            /usr/bin/vim.basic   30        manual mode
  4            /usr/bin/vim.tiny    15        manual mode

Press <enter> to keep the current choice[*], or type selection number:
```

输入你喜欢的编辑器的序号，然后回车即可
