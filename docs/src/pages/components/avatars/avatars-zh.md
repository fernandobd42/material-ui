---
title: React Avatar（头像）组件
components: Avatar, AvatarGroup, Badge
githubLabel: 'component: Avatar'
---

# Avatar 头像组件

<p class="description">在整个 material design 中，无论是在表格中还是到对话框菜单中，都可以找到使用头像的身影。</p>

{{"component": "modules/components/ComponentLinkHeader.js"}}

## 图片头像

通过将标准 `img` 的属性 `src` 或 `srcSet` 传递到组件中，您可以创建图片头像。

{{"demo": "pages/components/avatars/ImageAvatars.js"}}

## 字母头像

通过传入一个作为 `children`的字符串，您可以创建包含简单字符的头像组件。

{{"demo": "pages/components/avatars/LetterAvatars.js"}}

你可以为头像添加不同的背景颜色 下面的例子演示了如何通过人物的姓名来展示头像

{{"demo": "pages/components/avatars/BackgroundLetterAvatars.js"}}

## 尺寸

你可以通过改变 `height` 以及 `width` 这两个 CSS 属性来改变头像组件的尺寸。

{{"demo": "pages/components/avatars/SizeAvatars.js"}}

## 图标头像

通过将图标作为 `children` 来传递来创建图标头像。

{{"demo": "pages/components/avatars/IconAvatars.js"}}

## 其他的方式

如果你需要矩形或圆角的头像组件，请使用 `variant`属性。

{{"demo": "pages/components/avatars/VariantAvatars.js"}}

## 回调函数

如果在加载头像组件时发生错误，组件将按照如下顺序切换到以下备选方案：

- 提供的 children 子元素
- `alt` 文本的首字母
- 一个通用头像图标组件

{{"demo": "pages/components/avatars/FallbackAvatars.js"}}

## 分组

`AvatarGroup` renders its children as a stack. Use the `max` prop to limit the number of avatars.

{{"demo": "pages/components/avatars/GroupAvatars.js"}}

### Total avatars

If you need to control the total number of avatars not shown, you can use the `total` prop.

{{"demo": "pages/components/avatars/TotalAvatars.js"}}

## 带有徽章的组件

{{"demo": "pages/components/avatars/BadgeAvatars.js"}}
