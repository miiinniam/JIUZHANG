<div align="center">

<img src="https://img.shields.io/badge/玖章-JiuZhang-B42318?style=for-the-badge&labelColor=1547A8" alt="玖章" />

# 玖章 · JiuZhang

### 一枚朱砂落纸，让契约立此为凭

**专业的本地 PDF 电子签章工具 · 全程浏览器本地处理 · 零上传 · 零存储**

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Version](https://img.shields.io/badge/version-v2.0-B42318.svg)](#)
[![Platform](https://img.shields.io/badge/platform-Web-1547A8.svg)](#)
[![Single File](https://img.shields.io/badge/single-HTML-22c55e.svg)](#)
[![Made with](https://img.shields.io/badge/made%20with-❤️%20by%20Fayy-ff69b4.svg)](#)

</div>

---

## ✨ 项目简介

**玖章（JiuZhang）** 是一款**纯前端、单 HTML 文件**的 PDF 电子签章工具。打开浏览器即可使用，**所有 PDF 与印章数据从不离开你的设备**，特别适合处理合同、协议、报告等敏感文档的盖章场景。

> 「玖」即JIUNENG，章为印；玖章，意为九重契约，珍重所托。

## 🎯 项目亮点

- 🛡️ **隐私至上** — 100% 浏览器本地处理，无任何后端，无任何上传请求
- 📄 **零依赖部署** — 单个 HTML 文件，双击即用，可放进 U 盘随身携带
- 🎨 **专业签章效果** — 圆/椭圆/方形/姓名章/文字签名 5 种形态，4 向骑缝章
- ⚡ **生产力工具** — 批量盖章、水印平铺、章压字层级自动管理
- 🌗 **优雅交互** — 中式典雅 UI，支持暗色模式，完整快捷键

## 🚀 功能一览

### 🖋 签字与印章
- **手写签名**：可调笔触粗细 / 颜色，签名平滑
- **印章上传**：拖拽或点击导入 PNG / JPG / WebP
- **印章库持久化**：localStorage 自动保存，下次打开仍在
- **印章库导入 / 导出**：JSON 备份，跨设备迁移
- **智能扣章**：算法自动去除白边，容差实时预览

### 🎨 印章制作（v2.0 新增）
- **圆形章** — 标配公司印章，环形文字 + 五角星
- **椭圆章** — 部门 / 业务专用章
- **方形章** — 古风私章，自适应排版
- **姓名章** — 1~4 字方形 / 圆形朱印
- **文字签名生成** — 输入姓名 + 选书法字体（5 种），不会写字也能"签"

### 📐 签章操作
- **加签字 / 加印章** — 从库选取，一键放置
- **加文字 / 日期** — 7 种日期格式 + 自定义日期 + 自由文本批注
- **骑缝章** — 右 / 左 / 顶 / 底四向，混排页面自适应，可加随机错位
- **批量盖章**（v2.0）— 全部 / 范围 / 仅奇数页 / 仅偶数页 + 5 种放置位置
- **水印**（v2.0）— 文字水印，可旋转，可平铺整页，可调透明度
- **每页加** — 当前页元素一键复制到所有页

### 🎚️ 属性面板
- 位置 / 缩放 / 旋转 / **透明度**
- **9 宫格快速吸附**（四角 / 四边 / 居中）
- 章压字层级（签字层 / 印章层）
- 上移 / 下移图层

### 🛠️ 系统功能
- **撤销 / 重做**（最多 30 步）
- **缩放**（适配 / 100% / Ctrl+滚轮 / Ctrl±）
- **页面缩略图导航**
- **暗色模式**（v2.0 · `Ctrl+/`）
- **完整快捷键面板**

## ⌨️ 快捷键

| 操作 | 快捷键 |
|---|---|
| 撤销 | `Ctrl + Z` |
| 重做 | `Ctrl + Y` |
| 复制选中 | `Ctrl + D` |
| 删除选中 | `Delete` |
| 放大 / 缩小 | `Ctrl + +` / `Ctrl + -` |
| 适配窗口 | `Ctrl + 0` |
| 滚轮缩放 | `Ctrl + 滚轮` |
| 切换主题 | `Ctrl + /` |
| 关闭弹窗 | `Esc` |

## 🚀 快速开始

### 方式一：直接下载使用（推荐）

```bash
# 下载仓库
git clone https://github.com/<your-user>/JiuZhang.git
cd JiuZhang

# 双击打开即可，无需任何安装
open "玖章 - 本地PDF电子签章工具v2.0.html"
```

### 方式二：在线使用

部署到任意静态托管即可：GitHub Pages / Vercel / Netlify / Cloudflare Pages 都行。

```bash
# 例如用 Python 起一个本地静态服务
python3 -m http.server 8080
# 然后浏览器访问 http://localhost:8080
```

### 方式三：嵌入到自己的项目

整个工具就是一个 HTML 文件，复制走即可。所有外部依赖通过 CDN 引入，无需 npm install。

## 🧰 技术栈

纯前端，无构建工具，无框架：

| 技术 | 用途 |
|---|---|
| [PDF.js](https://mozilla.github.io/pdf.js/) | PDF 解析与页面渲染 |
| [pdf-lib](https://pdf-lib.js.org/) | PDF 写回与导出 |
| [Fabric.js](http://fabricjs.com/) | 画布元素管理（拖拽/缩放/旋转） |
| [Signature Pad](https://github.com/szimek/signature_pad) | 手写签名 |
| [Tailwind CSS (CDN)](https://tailwindcss.com/) | 样式 |

> 🌟 **零构建依赖**：没有 `package.json`，没有 `node_modules`，没有打包步骤。

## 🌐 浏览器兼容

| 浏览器 | 支持 |
|---|---|
| Chrome / Edge | ✅ 完美支持（推荐） |
| Safari | ✅ 完美支持 |
| Firefox | ✅ 完美支持 |
| 移动端浏览器 | ✅ 响应式适配，触屏可用 |

需要现代浏览器（支持 Canvas / FileReader / localStorage）。

## 🛡️ 隐私声明

> **本工具不会发送任何 PDF 或印章数据到服务器。**

- ❌ 没有后端服务
- ❌ 没有任何 `fetch` / `XMLHttpRequest` 请求（除 CDN 加载库本身）
- ❌ 没有埋点 / 没有统计 / 没有日志上报
- ✅ 所有数据存储在 `localStorage`（仅本机）
- ✅ 关闭浏览器或清空缓存即可彻底删除

担心 CDN？可以把所有 `<script src>` 替换为本地路径（在 `head` 里）。

## 📸 功能截图

> 截图可放置于 `docs/screenshots/` 目录后引用：

```
docs/screenshots/
├── hero.png        # 封面
├── editor.png      # 编辑器
├── stamp-maker.png # 印章制作
├── dark-mode.png   # 暗色模式
└── batch-stamp.png # 批量盖章
```

## 🗺️ 路线图

- [ ] 数字签名（PKI / 证书签名）
- [ ] PDF 表单填写
- [ ] PDF 拆分 / 合并
- [ ] 国际化（i18n）支持
- [ ] PWA 离线版本
- [ ] OCR 自动定位"盖章处"

欢迎 issue / PR！

## 🤝 贡献

发现 bug 或想加新功能？

1. Fork 本仓库
2. 创建分支 `git checkout -b feature/my-feature`
3. 提交 `git commit -m 'feat: add my feature'`
4. 推送 `git push origin feature/my-feature`
5. 提个 Pull Request

## 📜 License

[MIT License](LICENSE) · 你可以自由使用、修改、分发本项目代码。

## ⚠️ 免责声明

> **本项目仅供学习与个人使用**，所生成的电子印章不具备法律效力。
> 商业 / 法律场景下的合同盖章请使用具备 **CA 数字证书** 的合规电子签名服务。
> 因不当使用本工具造成的任何损失，作者不承担任何责任。

## 💖 致谢

- 感谢 [PDF.js](https://github.com/mozilla/pdf.js) / [pdf-lib](https://github.com/Hopding/pdf-lib) / [Fabric.js](https://github.com/fabricjs/fabric.js) / [Signature Pad](https://github.com/szimek/signature_pad) 等优秀开源项目
- 感谢每一位 star 和 fork 的朋友 ⭐
- 「玖章」之名，取「九重契约，珍重所托」之意

---

<div align="center">

**如果这个项目对你有帮助，欢迎点亮 ⭐ Star 支持一下**

Made with ❤️ for everyone who values privacy.

</div>
