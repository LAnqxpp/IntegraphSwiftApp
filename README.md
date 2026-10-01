# 桌球计分器 · 上架网页

静态站点，可直接托管到任意 HTTPS 空间（GitHub Pages / Cloudflare Pages / 自有域名等）。

## 页面

| 文件 | 用途 | App Store Connect 对应项 |
|------|------|--------------------------|
| `index.html` | 技术支持 | Support URL（技术支持网址） |
| `privacy.html` | 隐私政策 | Privacy Policy URL |
| `terms.html` | 用户协议 | 可选，可放在描述或支持页 |

## 本地预览

```bash
cd AppStoreAssets/Website
python3 -m http.server 8080
```

浏览器打开：http://127.0.0.1:8080/

## 部署示例（GitHub Pages）

1. 新建公开仓库，例如 `zhuoqiu-jifenqi-site`
2. 将本目录下全部文件推送到仓库根目录（或 `docs/`）
3. 仓库 Settings → Pages → 启用 GitHub Pages
4. 得到类似地址：
   - 技术支持：`https://你的用户名.github.io/zhuoqiu-jifenqi-site/`
   - 隐私政策：`https://你的用户名.github.io/zhuoqiu-jifenqi-site/privacy.html`
   - 用户协议：`https://你的用户名.github.io/zhuoqiu-jifenqi-site/terms.html`

## 上架前请修改

- 把 `support@zmkjchat.com` 换成你真实可用的支持邮箱（三个 HTML 均需改）
- 确认域名可公网 HTTPS 访问后再填入 App Store Connect
