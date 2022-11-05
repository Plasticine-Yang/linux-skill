# 安装 rust

在国内运行`rust`官方的安装命令不可行，需要设置镜像源

```shell
nvim ~/.zshrc

# 配置这两个环境变量
export RUSTUP_UPDATE_ROOT=https://mirrors.ustc.edu.cn/rust-static/rustup
export RUSTUP_DIST_SERVER=https://mirrors.ustc.edu.cn/rust-static
```

然后再执行官方的安装脚本:

```shell
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```
