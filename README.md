# gpui-pre (Tabby RS)

Tabby RS 使用的 [gpui-pre](https://crates.io/crates/gpui-pre) 修改版，gpui-pre 是 [Zed](https://github.com/zed-industries/zed) 中 GPUI 的快照

本仓库只含需要修改的包，其余 `gpui-pre-*` 包仍从 crates.io 取：

```
gpui-pre/           # gpui-pre 0.3.12
gpui-pre-linux/     # gpui-pre-linux 0.3.12
gpui-pre-windows/   # gpui-pre-windows 0.3.12
```

第一个提交是 crates.io 上 0.3.12 的原样源码，之后每个提交是一处修复

## 使用

在依赖方的 `Cargo.toml` 中替换 crates.io 的包：

```toml
[patch.crates-io]
gpui-pre = { git = "https://github.com/tabby-rs/gpui-pre", tag = "<标签>" }
gpui-pre-linux = { git = "https://github.com/tabby-rs/gpui-pre", tag = "<标签>" }
gpui-pre-windows = { git = "https://github.com/tabby-rs/gpui-pre", tag = "<标签>" }
```

## 许可

与上游相同，Apache-2.0，见各包目录的 `LICENSE-APACHE`
