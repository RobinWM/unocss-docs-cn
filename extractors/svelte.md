---
title: UnoCSS Svelte 提取器指南 - 从 class: 指令中提取类
description: 学习如何使用 UnoCSS Svelte 提取器，从 class: 指令中提取类并生成相应的 CSS，提升开发效率。
head:
  - - meta
    - name: keywords
      content: UnoCSS, Svelte, 提取器, class 指令, CSS 生成
---

# Svelte 提取器

支持从 `class:` 指令中提取类。

```html
<div class:text-orange-400="{foo}" />
```

将被提取为 `text-orange-400` 并生成：

```css
.text-orange-400 {
  color: #f6993f;
}
```

## 安装

::: code-group

```bash [pnpm]
pnpm add -D @unocss/extractor-svelte
```

```bash [yarn]
yarn add -D @unocss/extractor-svelte
```

```bash [npm]
npm install -D @unocss/extractor-svelte
```

:::

```ts [uno.config.ts]
import extractorSvelte from '@unocss/extractor-svelte'
import { defineConfig } from 'unocss'

export default defineConfig({
  extractors: [extractorSvelte()]
})
```
