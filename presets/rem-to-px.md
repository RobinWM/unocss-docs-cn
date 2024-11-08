---
title: Rem to px 预设 - 将 rem 转换为 px
description: 为所有工具类将 rem 转换为 px (@unocss/preset-rem-to-px)，简化样式转换。
head:
  - - meta
    - name: keywords
      content: UnoCSS, Rem to px, 工具类, CSS, 前端开发
outline: deep
---

# Rem to px 预设

将所有工具类中的 rem 转换为 px。

[源代码](https://github.com/unocss/unocss/tree/main/packages/preset-rem-to-px)

## 安装

::: code-group

```bash [pnpm]
pnpm add -D @unocss/preset-rem-to-px
```

```bash [yarn]
yarn add -D @unocss/preset-rem-to-px
```

```bash [npm]
npm install -D @unocss/preset-rem-to-px
```

:::

```ts [uno.config.ts]
import presetRemToPx from '@unocss/preset-rem-to-px'
import { defineConfig } from 'unocss'

export default defineConfig({
  presets: [
    presetRemToPx()
    // ...other presets
  ]
})
```

## 使用方法

```html
<div class="m-2"></div>
```

::: code-group

```css [无]
.m-2 {
  margin: 0.5rem;
}
```

```css [有]
.m-2 {
  margin: 8px;
}
```

:::

## 选项

### baseFontSize

- **类型：** `number`
- **默认值：** `16`

将 rem 转换为 px 的基准字体大小 (`1rem = n px`)。
