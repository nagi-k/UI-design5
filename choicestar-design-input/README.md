# 择校星 ChoiceStar · Trae Design AI 画布输入包

本文件夹包含把「择校星 ChoiceStar」项目导入 Trae Design / AI 画布所需的全部材料。你可以直接把这些文字说明 + 原型文件 +（如有）界面截图一起提供给 AI，让它在画布中生成每个界面的高保真页面，下载后你再在 Figma 中微调。

## 文件夹结构

```
choicestar-design-input/
├── README.md                          # 本说明书
├── 00-how-to-use-trae-design.md       # 把材料喂给 Trae Design 的具体步骤
├── 01-project-brief.md                # 项目背景、目标用户、价值主张
├── 02-design-system.md                # 颜色、字体、间距、圆角、阴影等 tokens
├── 03-page-map.md                     # 10 个界面的信息架构与跳转关系
├── 04-interaction-notes.md            # 全局交互规则（导航、状态、动效）
├── pages/                             # 每个界面的详细设计规格
│   ├── 01-home.md
│   ├── 02-smart.md
│   ├── 03-unis.md
│   ├── 04-majors.md
│   ├── 05-assess.md
│   ├── 06-mock.md
│   ├── 07-compare.md
│   ├── 08-career.md
│   ├── 09-community.md
│   └── 10-profile.md
├── screenshot-guide.md                # 如何自己截取高保真界面图
├── prototype/                         # 可交互原型（HTML + JS）
│   ├── index.html
│   └── js/tailwindcss-cdn.js
└── assets/screenshots/                # 你生成的界面截图放这里
```

## 最核心的三份材料

1. **每个界面的高保真截图**（最重要）
   - 如果已有 PNG/JPG 界面图，请放到 `assets/screenshots/`
   - 如果没有，请看 `screenshot-guide.md`，用浏览器打开 `prototype/index.html` 逐页截图
   - AI 画布最吃"视觉参考"，有图效果会远好于纯文字

2. **设计系统文档** `02-design-system.md`
   - 颜色、字体、间距、组件样式，保证 AI 生成的 10 个页面风格一致

3. **页面规格文档** `pages/*.md`
   - 每个页面"画什么、放什么文案、什么数据、什么交互"
   - 配合截图使用，AI 能精准还原细节

## 推荐的投喂顺序

1. 先上传 `01-project-brief.md` + 几张核心界面截图
2. 让 AI 生成"首页"和"智能填报"两个页面，验证风格
3. 再依次上传其余页面截图 + 对应 `pages/xx.md`
4. 最后用 `02-design-system.md` 统一校对颜色和组件

## 注意事项

- 所有尺寸按 **1440px 桌面端 Web** 设计，响应式适配到 1280px / 768px / 375px
- 本项目是 **B/C 端混合型 Web 应用**，不是纯移动端 App
- 图标使用内联 SVG / Emoji，无外部图标库依赖
- 图片、头像、院校 Logo 等使用占位图或抽象图形即可，AI 可自动填充
