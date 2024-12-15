## 指定目录安装 npm 包

要在指定目录安装 npm 包，你可以使用 `--prefix` 选项：

```bash
npm install --prefix ./目标目录 <包名>
```

# 操作

## 安装t-get

在根目录中.npm-global文件中安装（"."代表隐藏文件）

```bash
npm install --prefix ~/.npm-global -g t-get
```

## 验证t-get安装

如果有tget文件便的安装成功

```bash
ls -l ~/.npm-global/bin/t-get
```

## 使用t-get下载磁力

```bash
~/.npm-global/bin/tget 'magnet:链接'
```

## 扩展

**指定下载目录**

```bash
~/.npm-global/bin/tget 'magnet:链接' -d /path/to/download
```

**限制下载速度**

```bash
~/.npm-global/bin/tget 'magnet:链接' --max-speed 1024K
```

**设置最大连接数**

```bash
~/.npm-global/bin/tget 'magnet:链接' --max-connections 10
```

- 使用 `tget --help` 查看完整帮助信息