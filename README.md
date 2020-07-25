# FoxKit Extension Enforce Rewrite URL

某些网络托管服务商将前缀用于环境变量，这使得 FoxKit 无法识别是否启用了 mod_rewrite。该扩展程序强制执行重写的 URL。

警告：仅当您的网址中没有 'index.php' 的情况下，才使用此扩展！

## Nginx 重写示例

```
location / {
    try_files $uri $uri/ /index.php?$args;
}
```

## License

[MIT](./LICENSE)
