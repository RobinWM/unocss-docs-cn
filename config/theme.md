---
title: UnoCSS 主题系统指南 - 深度定制你的样式
description: 了解 UnoCSS 主题系统的用法，如何在配置中设置主题属性，提升样式的灵活性与可维护性。
head:
  - - meta
    - name: keywords
      content: UnoCSS, 主题, Tailwind, Windi, 样式定制
---

# 主题

`UnoCSS` 也支持像 Tailwind / Windi 中的主题系统。在用户级别上，您可以在配置中指定 `theme` 属性，它将与默认主题进行深度合并。

## 用法

<!--eslint-skip-->

```ts
theme: {
  // ...
  colors: {
    'veryCool': '#0000ff', // class="text-very-cool"
    'brand': {
      'primary': 'hsla(var(--hue, 217), 78%, 51%)', //class="bg-brand-primary"
    }
  },
}
```

## 在 `rules` 中使用

在规则中使用主题：

```ts
rules: [
  [
    /^text-(.*)$/,
    ([, c], { theme }) => {
      if (theme.colors[c]) return { color: theme.colors[c] }
    }
  ]
]
```

一个例外是，UnoCSS 将 `breakpoints` 控制权完全留给用户。当提供自定义 `breakpoints` 时，默认值将被覆盖而不是合并。例如：

<!--eslint-skip-->

```ts
theme: {
  // ...
  breakpoints: {
    sm: '320px',
    md: '640px',
  },
}
```

目前，您只能使用 `sm:` 和 `md:` 断点变量。

`verticalBreakpoints` 与 `breakpoints` 相同，但用于垂直布局。
