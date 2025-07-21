# minigrep

一个极简的 Rust 命令行项目，用于在文件中查找包含指定字符串的行。

## 用法

```sh
cargo run -- <查询字符串> <文件路径>
```

- `<查询字符串>`：要搜索的内容。
- `<文件路径>`：要搜索的文件。

支持通过设置环境变量 `IGNORE_CASE` 实现忽略大小写搜索：

```sh
$env:IGNORE_CASE=1; cargo run -- <查询字符串> <文件路径>
```

## 示例

```sh
cargo run -- to poem.txt
```

## 主要文件说明
- `src/main.rs`：程序入口，负责参数解析和错误处理。
- `src/lib.rs`：核心逻辑，包括参数配置、文件读取和搜索实现。

## 依赖
- Rust 标准库

## 构建与运行

```sh
cargo build
cargo run -- <查询字符串> <文件路径>
```
