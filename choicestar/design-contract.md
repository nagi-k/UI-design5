# 择校星 ChoiceStar · Design Contract

## Tech stack
vanilla 单文件 SPA（index.html 内嵌 CSS+JS），Tailwind 经 CDN 引入（用户明确指定），emoji/内联 SVG 图标（用户明确指定），pure-static 交付。路径：/workspace/choicestar/index.html

## Style tier
business-international × 科技感浅色；aesthetic：清爽数据驾驶舱 + 大厂落地页；tone：专业、可信、年轻、高密度但清晰。

## Tokens
- primary #2563EB / primary-deep #1E3A8A / accent-orange #F97316 / green #10B981 / yellow #F59E0B / red #EF4444
- bg #F8FAFC / surface #FFFFFF / ink #0F172A / text-sub #64748B / border #E2E8F0
- font: "PingFang SC","Microsoft YaHei","Noto Sans SC",system-ui；display 同族 800 权重
- radius: 8/12/16；shadow 分层克制；spacing 4px 基；layout max-w-[1280px]
- motion: 页面切换 fadeUp 300ms ease-out；卡片 hover -4px；数字滚动；SVG 描边绘制；流光进度条
- bg-texture: Hero 网格 + 粒子连线 canvas + 渐变光斑

## App Shell（冻结）
固定顶部 nav（h-16，滚动后毛玻璃）：Logo + 10 导航项（home/smart/unis/majors/assess/mock/compare/career/community/profile）+ 搜索 + 省份 + 铃铛(badge) + 登录。
active 规则：data-nav 匹配路由加 .nav-active。main#page-root 渲染页模板；全局：AI 助手、Toast、模态框、回到顶部。

## Pages
home | smart | unis | majors | assess | mock | compare | career | community | profile（职责见 PRD）

## Mock schema
universities[10] / majors[10] / smartResult 冲稳保 / assessment 4×8题 / posts / lives / qa / news / testimonials / timeline / state{favorites, volunteerList, savedPlans, reports}
