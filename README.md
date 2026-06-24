# 减脂日历 App

一个可在手机"安装到主屏幕"、离线可用的减脂食谱打卡 Web App(PWA)。

## 在线访问
https://diet.sunweiyong.asia

## 功能
- 一周菜单(标准日 / 拉面日 / 烧烤日)
- A/B/C 晚餐方案每天可切换
- 实时蛋白进度 + 缺口统计
- 体重记录打卡
- 全程离线可用,数据存在本机

## 本地预览
```
cd dietapp
python -m http.server 8000
# 浏览器打开 http://localhost:8000
```

## 部署到 GitHub Pages
1. 本仓库 → Settings → Pages
2. Source 选 `Deploy from a branch`
3. Branch 选 `main` / `(root)` → Save
4. 仓库根目录放 `CNAME` 文件名(内容为自定义域名)
5. 去域名服务商加 CNAME 解析指向 `<user>.github.io`

## 文件结构
```
dietapp/
├── index.html       # App 主体
├── manifest.json    # PWA 安装清单
├── sw.js            # Service Worker(离线缓存)
├── CNAME            # 自定义域名绑定(diet.sunweiyong.asia)
├── icon-192.png
├── icon-512.png
├── icon-192-maskable.png
├── icon-512-maskable.png
└── icon.svg
```
