# 📄 PDF 工具箱

一个纯前端的 PDF 处理工具，支持**合并、拆分、提取、删除、旋转** PDF 文件。所有处理均在本地浏览器完成，文件不会上传到任何服务器。

👉 **[立即使用](https://YOUR_USERNAME.github.io/pdf-toolbox)**

## 🔧 功能

| 工具           | 说明                                               |
| -------------- | -------------------------------------------------- |
| 🔗 **合并 PDF** | 上传多个 PDF，拖拽排序后合并为一个文件             |
| ✂️ **拆分 PDF** | 按每页拆分或自定义页码范围拆分，多页自动打包为 ZIP |
| 📋 **提取页面** | 预览缩略图，勾选需要的页面导出为新 PDF             |
| 🗑️ **删除页面** | 预览缩略图，勾选要删除的页面后导出                 |
| 🔄 **旋转页面** | 选择页面旋转 90°/180°/270°，支持逐页不同角度       |

## 🚀 部署到 GitHub Pages

### 第一步：创建仓库

1. 在 GitHub 上创建一个新仓库，命名为 `pdf-toolbox`（或任意名称）
2. 设置为 **Public**（公开）
3. 不要勾选 "Add a README file"

### 第二步：上传文件

```bash
git clone https://github.com/YOUR_USERNAME/pdf-toolbox.git
cd pdf-toolbox

# 将 index.html 复制到仓库目录
cp /path/to/index.html .

git add index.html
git commit -m "Initial commit: PDF toolbox"
git push origin main
```

### 第三步：启用 GitHub Pages

1. 打开仓库 → **Settings** → **Pages**
2. **Source** 选择 `Deploy from a branch`
3. **Branch** 选择 `main`，文件夹选 `/ (root)`
4. 点击 **Save**
5. 等待 1-2 分钟，页面链接会显示在顶部

### 第四步：分享链接

部署完成后，你的链接格式为：

```
https://YOUR_USERNAME.github.io/pdf-toolbox
```

直接把这个链接发给微信好友，他们在微信里点开就能用！

## 🔒 隐私说明

- 所有 PDF 文件的读取、处理、下载均在**你的浏览器本地**完成
- **不会**上传到任何服务器
- **不需要**注册或登录
- 完全离线可用（首次加载后会缓存 CDN 资源）

## 🛠 技术栈

- [pdf-lib](https://github.com/Hopding/pdf-lib) — PDF 生成与修改
- [pdf.js](https://github.com/mozilla/pdf.js) — PDF 页面渲染（缩略图预览）
- [JSZip](https://github.com/Stuk/jszip) — ZIP 打包（拆分多文件时）

所有依赖通过 CDN 加载，无需安装或构建。

## 📱 兼容性

- ✅ Chrome / Edge (桌面 & 移动端)
- ✅ Safari (iPhone / iPad / Mac)
- ✅ 微信内置浏览器
- ✅ Firefox

> 建议使用 2020 年后发布的浏览器版本以获得最佳体验。
