# Cat Maven 影视订阅源 v2

## 文件
- `index.main.json`：Cat Maven 订阅入口清单。
- `plugins/json/`：从 Cat-Maven-2023 原项目复制的 Mac 采集配置。
- `resource-sites-catalog.json`：从 awesome-zhuiju-free 的 resources/resources.json 整理的在线影视网站参考目录。

## 本版整理规则
- 只纳入原 Cat Maven 项目清单中 `engineType: Mac` 且 JSON 文件确实存在的配置，共 35 个。
- 不把普通网站首页、TVBox 配置地址或磁力搜索站误当成 Cat Maven 的 Mac API。
- 资源目录保留站点验证状态，`removed` / `caution` 不是可用性保证。
- 所有配置继承自所提供的 Cat Maven 项目；本次未进行联网接口测试，也不保证播放可用性。

## 导入方式
将整个目录部署到支持静态文件的 HTTPS 托管服务，并确保 `index.main.json` 与 `plugins/` 位于同一根目录。然后在 Cat Maven 中添加该 `index.main.json` 的公网 HTTPS 地址。仅在本地时可先用 JSON 检查结构，但相对下载地址需要服务端根目录正确。
