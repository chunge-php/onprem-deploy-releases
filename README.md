# onprem-deploy-releases

**这个仓库是故意公开的**,只放版本清单(和可选的升级包 zip),不放任何源码。

客户机器的升级脚本从这里检查新版本:

```
https://raw.githubusercontent.com/chunge-php/onprem-deploy-releases/main/version.json
```

## 发布新版本

改 `version.json` 的 `latest` / `changelog` / `bundle_url`,提交推送即可(raw CDN 缓存约 1-5 分钟后全球生效)。

- `mandatory: false` → 客户可以选择不升级
- `channels` → 按客户钉不同版本
- 升级包 zip 可直接放本仓库(注意里面的迁移 SQL 会公开),介意就放自己服务器
