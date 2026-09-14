# 02 · 设计系统 Design System

## 颜色 Tokens

| Token | 色值 | 用途 |
|-------|------|------|
| Primary | `#4C6EF5` | 主按钮、链接、选中状态、关键数据 |
| Primary Light | `#EAF1FF` | 浅色背景、hover 背景 |
| Primary Dark | `#364FC7` | 按钮按下、强调文字 |
| Accent | `#38BDF8` | 装饰性强调、图表、高亮 |
| Background | `#F8FAFC` | 页面背景 |
| Surface | `#FFFFFF` | 卡片、弹窗、输入框背景 |
| Border | `#E5E7EB` | 分割线、卡片边框 |
| Text Main | `#111827` | 主标题、正文 |
| Text Sub | `#6B7280` | 次要说明、辅助文字 |
| Text Muted | `#9CA3AF` | 占位符、禁用文字 |
| Success | `#22C55E` | 成功、安全、录取概率高 |
| Warning | `#F59E0B` | 警告、中等风险、冲一冲 |
| Danger | `#EF4444` | 错误、高风险、保底 |
| Info | `#3B82F6` | 信息提示 |

## 字体

- 中文字体：`"PingFang SC", "Microsoft YaHei", "Noto Sans SC", sans-serif`
- 英文字体：`"Inter", "SF Pro Display", -apple-system, BlinkMacSystemFont, sans-serif`
- 等宽数字：`"SF Mono", "DIN Alternate", monospace`

## 字阶

| 级别 | 大小 | 字重 | 用途 |
|------|------|------|------|
| H1 | 32px | 700 | 页面大标题 |
| H2 | 24px | 600 | 区块标题 |
| H3 | 18px | 600 | 卡片标题 |
| Body | 14px | 400 | 正文 |
| Caption | 12px | 400 | 辅助说明、标签 |
| Small | 11px | 400 | 时间、极小标签 |

## 间距系统

基础单位 4px：4 / 8 / 12 / 16 / 20 / 24 / 32 / 40 / 48 / 64

## 圆角

| Token | 值 | 用途 |
|-------|-----|------|
| sm | 8px | 小按钮、标签 |
| md | 12px | 按钮、输入框 |
| lg | 16px | 卡片、弹窗 |
| full | 999px | 胶囊标签、头像 |

## 阴影

```css
--shadow-sm: 0 1px 2px rgba(0,0,0,0.04);
--shadow-md: 0 4px 12px rgba(0,0,0,0.06);
--shadow-lg: 0 8px 30px rgba(0,0,0,0.08);
--shadow-float: 0 12px 40px rgba(76,110,245,0.16);
```

## 按钮规范

| 类型 | 背景 | 文字 | 圆角 | 高度 |
|------|------|------|------|------|
| Primary | `#4C6EF5` | 白色 | 12px | 40px |
| Secondary | 白色 + 边框 `#E5E7EB` | `#111827` | 12px | 40px |
| Text | 透明 | `#4C6EF5` | - | - |
| Tag | `#EAF1FF` | `#4C6EF5` | 999px | 24px |

## 卡片规范

- 背景：`#FFFFFF`
- 圆角：16px
- 内边距：20-24px
- 边框：1px solid `#E5E7EB` 或不带边框仅用阴影
- Hover：轻微上移 + 阴影加深

## 图标

- 使用内联 SVG 或 Emoji 占位
- 图标尺寸：16px / 20px / 24px
- 图标颜色与文字层级一致

## 图表规范

- 折线图：Primary 实线 + 数据点
- 柱状图：Primary 渐变
- 环形图：Primary / Accent / Success / Warning 分段
- 雷达图：Primary 填充 + 网格线
