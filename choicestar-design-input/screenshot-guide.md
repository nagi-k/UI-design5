# 截图指南 · 如何生成高保真界面图

## 推荐工具
- Chrome 浏览器
- 浏览器自带「开发者工具 → 运行命令 → Capture full size screenshot」
- 或任何截图工具：Snipaste、CleanShot、Figma 插件 Full Page Screen Capture

## 步骤

1. 启动本地服务器
```bash
cd choicestar-design-input/prototype
python3 -m http.server 8080
```

2. 用 Chrome 打开 `http://localhost:8080/`

3. 打开「开发者工具」（F12）

4. 按 `Ctrl+Shift+P`（Mac `Cmd+Shift+P`），输入 `Capture full size screenshot`，回车
   - 这会截取当前整个页面，包括滚动区域

5. 每个页面截图后保存为：
   - `assets/screenshots/home.png`
   - `assets/screenshots/smart.png`
   - `assets/screenshots/unis.png`
   - `assets/screenshots/majors.png`
   - `assets/screenshots/assess.png`
   - `assets/screenshots/mock.png`
   - `assets/screenshots/compare.png`
   - `assets/screenshots/career.png`
   - `assets/screenshots/community.png`
   - `assets/screenshots/profile.png`

6. 如果只想截取首屏，调整窗口宽度为 1440px，直接截图即可

## 截图尺寸建议
- 桌面端：1440 × 900（首屏）或 1440 × 全页高度
- 移动端：375 × 812

## 提示
- 截图前关闭浏览器插件、书签栏
- 保持 100% 缩放，不要缩放页面
- 如果页面有 fixed 元素遮挡，可用 DevTools 设备模拟模式
