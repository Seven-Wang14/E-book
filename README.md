# PDF E-book Reader(Chinese-English)
PDF电子书阅读器（中-英）

## Introduction | 项目简介
### 中文
这是一款基于 PDF.js 开发的纯前端PDF电子书阅读器，无需后端服务，仅依靠静态网页即可运行。程序自动适配电脑端与移动端设备，具备翻页、页码跳转、键盘快捷键、底部控制栏折叠等阅读功能。PDF文件会自动等比例缩放并高清渲染，界面带有阴影与毛玻璃效果，阅读界面简洁清爽。

### English
This is a pure front-end PDF e-book reader built with PDF.js. No backend server is required; it works simply as a static webpage.
The program automatically adapts to desktop and mobile devices, supporting page turning, page jump, keyboard shortcuts, and collapsible bottom control bar.
PDF files are scaled proportionally and rendered sharply. The UI is equipped with shadow and frosted glass effects to provide a clean reading environment.

---

## Core Features | 核心功能
### 中文
1. **自适应高清渲染**
PDF自动适配窗口尺寸，按照设备像素比高清绘制，画面不会拉伸模糊。
2. **双端设备适配**
电脑端显示左右侧边翻页按钮，移动端自动隐藏侧边按钮，适配手机屏幕。
3. **多样化翻页方式**
- 点击按钮切换上一页、下一页
- 输入页码一键直达目标页面
- 电脑端支持键盘快捷键：方向键、PageUp/PageDown、Home（首页）、End（末页）
4. **可折叠工具栏**
底部控制栏能够收起，只保留呼出按钮，最大化阅读可视区域。
5. **渲染队列优化**
快速连续翻页时自动排队等待渲染，防止页面卡顿、重复刷屏。
6. **开源信息弹窗**
点击按钮弹出开源说明，点击关闭按钮或者遮罩空白处都可以关闭弹窗。
7. **响应式布局**
手机端自动缩小控件间距，布局紧凑美观。

### English
1. **Adaptive high-definition rendering**
PDF fits the window automatically and renders sharply according to device pixel ratio without distortion.
2. **Cross-device adaptation**
Left and right page buttons are displayed on desktop and hidden automatically on mobile phones.
3. **Multiple navigation methods**
- Switch pages by clicking buttons
- Jump to the specified page by entering page number
- Desktop keyboard shortcuts: arrow keys, PageUp/PageDown, Home (first page), End (last page)
4. **Collapsible toolbar**
The bottom control bar can be folded to maximize reading area with a trigger button reserved.
5. **Render task queue optimization**
Avoid lag and repeated redraws when flipping pages rapidly.
6. **Open-source popup modal**
Click to open the introduction window; close it via button or clicking the mask area.
7. **Responsive layout**
Control elements will be compacted automatically on mobile screens.

---

## Tech Stack | 技术栈
### 中文
- 核心解析库：PDF.js（通过CDN引入，无本地依赖）
- 页面结构：原生 HTML
- 样式：CSS3（Flex布局、毛玻璃滤镜、过渡动画、媒体查询）
- 交互脚本：原生 JavaScript

### English
- Core library: PDF.js (loaded from CDN, no local dependencies)
- Markup: Native HTML
- Style: CSS3 (Flex layout, backdrop-filter, transition animation, media query)
- Script: Vanilla JavaScript

---

## Usage | 使用方法
### 中文
1. 将PDF电子书重命名为 `book.pdf`，和HTML文件放在同一个文件夹内。
2. 直接用浏览器打开HTML文件即可开始阅读。
3. 部署到 GitHub Pages 或者静态服务器时，仅需上传HTML文件与PDF文件，不需要配置后端。

> 提示：直接以 `file://` 本地打开时部分浏览器会触发跨域限制，建议使用本地静态服务或者部署到线上网页。

### English
1. Rename your PDF file to `book.pdf` and place it together with the HTML file.
2. Open the HTML file directly in the browser to start reading.
3. When deploying to GitHub Pages or static web server, just upload the HTML and PDF file. Backend configuration is not required.

> Note: Browsers may block local PDF access under `file://` protocol. Use a local static server or host the file online.

---

## File Structure | 文件结构
ebook-reader/
├── index.html # 阅读器主页面
└── book.pdf # 你的电子书文件

---

## Customization | 自定义修改
### 中文
1. 更换电子书：修改代码中 `PDF_FILE = 'book.pdf'` 为你的PDF文件地址。
2. 美化界面：修改CSS中的颜色、圆角、阴影、毛玻璃透明度。
3. 修改弹窗：编辑弹窗内的文字与GitHub链接。
4. 调整控件大小，适配更多屏幕尺寸。

### English
1. Change PDF file: Modify `PDF_FILE = 'book.pdf'` to your own PDF path.
2. Custom appearance: Adjust color, border radius, shadow and frosted transparency in CSS code.
3. Edit popup content: Change text and GitHub link inside modal box.
4. Resize buttons and text for more screen sizes.

---

## License
MIT License

You are free to use, modify and distribute this project for personal study and non-commercial purposes.
保留开源声明，可自由学习、二次修改。

This HTML file is developed for the E-book *Hanzhang*&*Poxiao-Fenghuoshihun*.
此次html用于编写电子书《含章》《破晓·烽火诗魂》

---

Wangjunchi
王俊驰
2026.6.26

