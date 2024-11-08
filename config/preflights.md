---
title: UnoCSS 预检功能指南 - 注入原始 CSS 以增强样式
description: 了解 UnoCSS 的预检功能，学习如何注入原始 CSS 作为预处理并利用主题自定义样式。
head:
  - - meta
    - name: keywords
      content: UnoCSS, 预检, 原始 CSS, 主题, 自定义样式
---

# 预检

您可以从配置中注入原始 css 作为预处理。解析的 `theme` 可用于自定义 css。

<!--eslint-skip-->

```ts
preflights: [
  {
    getCSS: ({ theme }) => `
      * {
        color: ${theme.colors.gray?.[700] ?? '#333'};
        padding: 0;
        margin: 0;
      }
    `
  }
]
```
