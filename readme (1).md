&lt;div align=&quot;center&quot;&gt;

# KotonohaShiori · 言叶之栞

**面向日音爱好者与译者的日文歌词振假名与双语明朝体排版工坊**

[version](https://www.google.com/search?q=https://github.com/your-username/kotonoha-no-shiori/releases)
[platform](https://www.google.com/search?q=https://github.com/your-username/kotonoha-no-shiori)
[built with](https://www.google.com/search?q=https://github.com/your-username/kotonoha-no-shiori)
[downloads](https://www.google.com/search?q=https://github.com/your-username/kotonoha-no-shiori/releases)

[English](https://www.google.com/search?q=README_EN.md) | [中文](README.md) | [日本語](https://www.google.com/search?q=README_JA.md) | [Deutsch](https://www.google.com/search?q=README_DE.md) | [Changelog](CHANGELOG.md)

<br/>

&lt;img src=&quot;docs/assets/preview-qrcode.png&quot; width=&quot;220&quot; alt=&quot;言叶之栞 扫码体验与预览&quot; /&gt;

&lt;/div&gt;

## 📋 GitHub 居中头部与徽章源码（可直接粘贴至 GitHub）

> 提示：普通 Markdown 预览器会自动过滤外部 `shields.io` 徽章图片与 `<div align="center">` 居中标签。将下方代码块直接复制到 GitHub 仓库的 `README.md` 中，即可在 GitHub 页面呈现与参考图完全一致的**居中大标题 + 副标题 + 四联彩色徽章 (`version` / `platform` / `built with` / `downloads`) + 多语言切换栏 + 居中图片/二维码**效果：

```markdown
<div align="center">

# KotonohaShiori · 言叶之栞

**面向日音爱好者与译者的日文歌词振假名与双语明朝体排版工坊**

<p align="center">
  <img src="https://img.shields.io/badge/version-v2.4.0-007ec6" alt="version" />
  <img src="https://img.shields.io/badge/platform-Web%20%7C%20Mobile%20%7C%20Desktop-7a7a7a" alt="platform" />
  <img src="https://img.shields.io/badge/built%20with-Tailwind%20%2B%20Kuromoji-e06c40" alt="built with" />
  <img src="https://img.shields.io/badge/downloads-25k-3b9712" alt="downloads" />
</p>

<p align="center">
  <a href="./README_EN.md">English</a> |
  <a href="./README.md">中文</a> |
  <a href="./README_JA.md">日本語</a> |
  <a href="./README_DE.md">Deutsch</a> |
  <a href="./CHANGELOG.md">Changelog</a>
</p>

<p align="center">
  <img src="./docs/assets/qrcode.png" width="200" alt="QR Code / Preview" />
</p>

</div>
```

## ✨ 项目简介

**KotonohaShiori（言叶之栞）** 是一款专为日音爱好者、日语学习者与歌词译者打造的前端单文件 Web 排版工坊。项目以日系文库本与音乐杂志的**明朝体（Serif）排版美学**为核心，融合轻盈的二次元视觉元素，支持日文歌词自动振假名（Furigana）、送假名智能对齐、URL 网页歌词一键提取、点击式交互改音、全光谱自由取色，以及一键导出原生带注音的 **Microsoft Word (`.doc`)** 与独立网页文档。

## 🌟 核心特性

### 1. 典雅明朝体与双语排版系统
- **跨平台明朝体字体栈**：舞台展示区默认配置严谨的日文明朝体回退链（`Hiragino Mincho ProN` → `Yu Mincho` → `Source Han Serif JP` → `Noto Serif CJK JP` → `Songti SC`），内置 **7 款日文字体预设**与 **4 款中文译文字体模式**。
- **黄金比例 `<ruby>` 注音微调**：针对明朝体横细竖粗的笔画特征，将 `<rt>` 振假名字号默认设定为 `0.55em`（支持 `0.45em` ～ `0.70em` 多档调节），配合 `2.0` ～ `3.0` 防黏连行高，杜绝假名注音与上行文字发生纵向碰撞。
- **手输 + 预设一体式微调控件**：字体大小（`12px` ～ `72px`）与字间距（`-0.05em` ～ `0.50em`）均采用「左侧自由数值输入 + 右侧预设下拉秒切」的双联组合框设计。
- **全光谱自由取色与多主题切换**：支持通过原色圆点取色器自由定制**日文原文**、**振假名注音**、**中文译文**三层独立色彩，并提供 5 套快捷色盘（樱歌粉、星海蓝、言叶绿、暮光紫、古典朱墨）与 3 套全局主题（🌸 樱色二次元 / 📜 和纸浅色 / 🌙 水墨暗夜）。

### 2. 智能分词与交互式改音引擎
- **双引擎振假名解析**：内置高频日音歌词词典并静默挂载 `Kuromoji.js` 形态素解析器，自动识别汉字并生成 `<ruby>漢字<rt>かな</rt></ruby>` 结构。
- **送假名（Okurigana）边界对齐**：自动剥离词尾送假名（如将「悲しみ」精准拆分为 `<ruby>悲<rt>かな</rt></ruby>しみ`），避免整词笼统注音。
- **歌词特殊读音（当て字）语法支持**：支持在输入框中使用 `漢字(かんじ)`、`漢字（かんじ）` 或 `漢字《かんじ》` 语法直接指定特殊艺术读音（例如 `未来(あした)`、`運命(さだめ)`、`宇宙(そら)`）。
- **所见即所得点击改音**：直接点击预览舞台上的任意汉字或打开顶部「修改注音词表」抽屉，即可弹窗修改假名读音，支持选择**应用到全文同名词汇**、**仅修改当前所在行**或**一键移除注音**。

### 3. 🔗 URL 链接一键提取歌词
- **多源网页解析**：支持直接粘贴 **Uta-Net (歌ネット)**、**Utaten**、**J-Lyric**、**网易云音乐单曲链接**及通用日文歌词网页 URL，一键抓取曲名、歌手与歌词正文。
- **标签还原与双语自动分流**：自动将网页内置的 `<ruby>` 标签转化为可编辑的 `漢字(かな)` 格式，智能剔除 `.lrc` 时间轴标签（如 `[00:12.34]`）与作词作曲元数据，并自动识别「一日一中」交替文本，拆分为日文原词与中文译文两栏。

### 4. 多格式导出与响应式交互体验
- **一键生成 Word 文档 (`.doc`)**：无需后端服务，前端直接生成兼容 Microsoft Word 与 WPS 的 Print 视图文档，完整保留 `<ruby>` 双行注音结构、字号比例、对齐方式及自定义字体颜色。
- **HTML 与纯文本导出**：支持一键复制干净的 `<ruby>` HTML 代码片段、复制带括号注音的双语对照纯文本，或导出可离线浏览的独立 `.html` 排版文件。
- **二次元细节与移动端适配**：内置看板娘「栞音 (Shione)」互动提示、飘落樱花背景动效、统一 2×4 等高工作台网格、输入框独立 `✕` 快速清除按钮，以及针对手机端优化的「✏️ 歌词输入 / 📖 排版预览 / ✨ 修改注音」三栏切换导航。

## 🛠️ 技术栈与架构设计

| 模块分类 | 采用技术 / 方案 | 说明 |
| :--- | :--- | :--- |
| **核心框架** | Vanilla HTML5 + ES6+ JavaScript | 零构建依赖，单文件即开即用，易于部署或嵌入 |
| **样式系统** | Tailwind CSS (CDN) + CSS Variables | 基于 Design Tokens 统一管理主题色、字号、行高与卡片阴影 |
| **字体资源** | Google Fonts + 本地系统明朝体栈 | 集成 `Shippori Mincho`、`Noto Serif JP/SC`、`Klee One` 等字体 |
| **分词与注音** | 内置高频歌词词典 + `Kuromoji.js` | 首屏词典毫秒级直出，后台静默加载完整日文形态素词典 |
| **网页抓取解析** | `DOMParser` + 多节点 CORS Proxy | 自动降级轮询 `allorigins` / `corsproxy` / `jina.ai` 提取歌词正文 |
| **文档导出** | MSO Word HTML (`application/msword`) | 原生映射 `<ruby><rb>...<rt>...</ruby>` 至 Word 拼音指南结构 |

## 🚀 快速开始

```bash
# 1. 克隆仓库到本地
git clone https://github.com/your-username/kotonoha-no-shiori.git

# 2. 进入项目目录并直接在浏览器中打开
cd kotonoha-no-shiori
open furigana_mincho_studio.html
```

## 📐 核心排版规范参数

| 排版属性 | CSS 变量名 | 默认值 | 可调范围 / 说明 |
| :--- | :--- | :--- | :--- |
| **日文主字体栈** | `--font-jp` | `Hiragino Mincho ProN, Yu Mincho...` | 内置 7 套明朝体 / 手写体 / 圆体栈切换 |
| **中文译文字体栈** | `--font-zh` | `Songti SC, Noto Serif SC...` | 支持思源宋体、与日文同步、手写楷体、黑体 |
| **正文基准字号** | `--lyric-font-size` | `26px` | 支持 `12px` ～ `72px` 手动输入与 5 档预设 |
| **防碰撞行高** | `--lyric-line-height` | `2.45` | 支持 `2.0` ～ `3.0`，预留充足 `<rt>` 纵向空间 |
| **振假名字号比例** | `--ruby-font-scale` | `0.55em` | 支持 `0.45em` / `0.50em` / `0.55em` / `0.62em` / `0.70em` |
| **字间距** | `--lyric-letter-spacing` | `0.05em` | 支持 `-0.05em` ～ `0.50em` 无级调节 |
| **双语字号级差** | `--zh-font-scale` | `0.76` | 译文字号约为日文原文的 `76%`，层次分明 |

## 📄 开源协议

本项目基于 **MIT License** 开源，欢迎自由使用、修改与分享。