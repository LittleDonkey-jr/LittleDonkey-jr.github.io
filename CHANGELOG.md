# Change Log

## [1.0.3] - 2024-5-29

### Refactored

- 修复了一些在 **Accessibility** 上的问题
- 优化了部分内容，速度更快了

## [1.0.4] - 2024-5-30

### Refactored

- 优化了部分内容，评分 **395**
- 修改了 README

## [1.1.0] - 2024-6-2

### Features

- 新增 `ProjectCard`
- 完善了 Project 页面

### Refactored

- 取消了头图的懒加载，删去了莫名其妙的 br

## [1.1.1] - 2024-6-2

### Refactored

- 优化链接样式，在 `pagespeed.web` 获得 400 分

## [1.1.2] - 2024-6-12

### Features

- 新增 `busuanzi` 计数器

## [1.2.0] - 2024-6-16

### Features

- `css` 已经改为 `scss`
- 自定义了 `waline` 的样式
- 完善了 `Footnotes` 的样式
- 添加图标

## [1.2.1] - 2024-6-28

### Features

- 爆改 `scss` 文件，基本上改成了 `Tailwind`
- 修改了 `footer` 的样式

### Refactored

- 微调了部分组件的样式
- 微调了文章样式
- 删去了不必要的友链

## [2.0.0] - 2024-7-8

### Features

- `Lighthouse` 400
- 文本压缩……启动！！
- 页脚修改……返璞归真

### Refactored

- 删除 `busuanzi` 计数器

### Fix

- 修复了文章内标签跳转的问题

## [2.1.0] - 2024-7-9

### Features

- 新增搜索功能

### Refactored

- 微调页脚
- 微调导航栏

## [2.1.1] - 2024-7-9

### Fix

- 修复了不能跳转的问题（原因未知）

## [2.1.2] - 2024-7-10

### Features

- （半成品）添加 `twikoo` 评论
- 一些组件，将在 2.2.0 总结

### Refactored

- 完善了搜索的黑夜模式

## [2.2.0] - 2024-7-13

### Features

- 添加目录功能！（终于加了）
- 添加了一篇指导文章
- 添加了新的组件

### Refactored

- 修改了行距

### Fix

- 修复了在手机屏幕下页脚显示不全的问题

## [2.3.0] - 2024-7-18

### Features

- 添加了代码框的行号
- 提交了如何修改代码框主题的教程

### Refactored

- 修改了 `astro.config.mjs` 现在代码框样式完全了

## [2.3.1] - 2024-7-19

### Fix

- 修复了 `astro.config.mjs` 中的问题（我填错了位置了）
- 完善了白天的代码框样式

## [2.4.0] - 2024-7-21

### Refactored

- 更改了 `<main>` 的位置，现在它只包含 card 而不包含 footer
- 重写了有关**社交链接**、**菜单**、**导航栏**以及**评论**的 `.astro` 文件，现在它们通过 `consts.ts` 来生成其内容
- 把**社交链接**的 svg 与配置文件分离
- 删去了不必要的文件与 `import`

### Fix

- 修复了原 JS 文件中的一堆 error ，现在它们都有了防 null 判断而不会出错
- 指定了 page 与 post 的数据结构，现在不会报 never 错误了
- 修复了若干错误，现在项目可以通过 `npx astro check`

## [2.5.0-alpha] - 2024-7-22

### Features

- 新增返回顶部按钮
- 新增适用于平板的界面样式
- 新增文章、仓库卡片的样式
- 新增导航栏图标，适配平板样式
- 现在你可以通过 `consts.ts` 自定义主题中的辅助文字内容

### Refactored

- 全面重写页面，将原本的元素内滚动改成了通过 grid 搭建的页面，解决了无法平滑跳转、滚动条乱飞的问题。现在整个页面成为一个更紧密结合的整体
- 侧边栏重写，使用 sticky 定位，添加了图标
- 重写文章、仓库卡片的样式，现在文章的标题、简介不再会被隐藏而是会自动适应
- 重写文章、仓库卡片在小屏幕下的样式
- 重写按钮的样式，现在它们被集成到侧边栏中，而不是脱离于主页面
- 重写目录的样式，现在它会自动生成在侧边栏中

### Fix

- 修复了原 tag 文件中变量的命名问题
- 统一了 Astro.props 的格式（使用断言）
- 修复了文章标题、简介过长导致的溢出问题

## [2.5.0-alpha.2] - 2024-7-22

### Features

- 清理了 global.scss
- 为没有标签的文章自动添加了一个不可点击的未分类标签，视觉上更统一
- 为 collapse 与 diff 添加了 m-2 ，现在它们不会突出去了

### Refactored

- 全部改成 Tailwind

### Fix

- 修复了上一页、下一页按钮与页脚黏在一起的问题

## [2.5.0-alpha.3] - 2024-7-23

### Fix

- 修复了手机视图下导航栏消失不见的问题

## [2.5.0-alpha.4] - 2024-7-24

### Fix

- 修复了项目卡片无法获取信息的问题
- 修复了在博客、项目页面下目录跳转的问题

## [2.5.0-alpha.5] - 2024-7-26

### Fix

- 修复了项目卡片中错误的样式类
- 修复了有关于类型的问题，现已通过 check 0.8.2

## [2.5.0-beta] - 2024-7-29

### Features

- 现在行号和顶栏已经与代码分开且被固定
- 新增代码框显示语言的功能

### Refactored

- 重写了代码框的结构（使用 shiki 转换器）

### Fix

- 修复了在手机视图下卡片显得过小的问题

## [2.5.0-beta.2] - 2024-7-29

### Refactored

- 调整了一下代码框顶栏，现在元素垂直居中了
- 调整了在手机视图下卡片的 padding

### Fix

- 修复了文章跳转 target 错误的问题（为什么才发现这个严重问题）

## [2.5.0-beta.3] - 2024-7-30

### Features

- `consts.ts` 添加了标签页的配置，这是主名称
- `BaseLayout.astro` 添加了标签页的配置，现在你可以为每一个页面添加属于它自己的标签页名称

### Refactored

- 断言界定了 JS 中元素的类型，避免 TS 报错
- 调整了一下代码框结构，现在代码右侧与代码框有了一定的留白
- 调整了博客与项目页面的结构，统一 `mt-8` `mb-8`

### Fix

- 修复了昼夜切换按钮实际操作区域与显示区域不一致的问题
- 修复了昼夜切换按钮不同步的问题，现在两个按钮与其实际主题统一

## [2.5.0-rc] - 2024-8-1

### Features

- 常驻了上下页的按钮，这下大家就知道我的博客其实是有做分页的了
- 添加了分页的按钮，终于不用一页一页地跳了

### Refactored

- 单页页面改成了十篇文章
- 去掉了 layout 的 title

## [2.5.0] - 2024-8-2

### Features

- 添加分类功能，现在你可以为你的文章添加两个独立的索引：分类与标签
- 给分类与标签的文章列表页面添加了分页功能，不再是一整页了
- 在侧边栏集成了分类的功能，来自 issue #10

### Refactored

- 现在如果文章没有图片，它的文章信息将会填充
- 修改了分页按钮的样式
- 微调样式，来自 issue #9

### Fix

- 修复在文章过多时分页失效的问题
- 修复在 issue #11 中提到的问题

## [2.5.1] - 2024-8-4

### Features

- 修改了 README
- 添加了 Vercel Web Analytics （不使用 vercel 的用户需要注意一下）

### Refactored

- 改善了整体排版，现在段落之间更清楚了
- 修复了页脚一些奇怪的居中问题
- 更换了 Footnotes 的卡片颜色
- 删除了底部版权信息卡片的阴影
- 添加了表格每一行的分割线
- 把 `<code>` 的字体稍微改大了一点

## [2.5.2] - 2024-8-7

### Features

- 改进了 `TimeLine` 的格式，现在比之前方便多了
- 在侧边栏添加分类与标签卡片，移除原来的分类页面

### Refactored

- 修改了卡片样式
- 修改了链接样式
- 清理了原评论系统中不必要的代码

### Fix

- 修复了部分手机导航栏无法跳转的问题
