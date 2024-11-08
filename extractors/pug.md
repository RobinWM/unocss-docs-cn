---
title: UnoCSS Pug 提取器指南 - 从 Pug 模板中提取类
description: 了解 UnoCSS 的 Pug 提取器 (@unocss/extractor-pug)，学习如何从 Pug 模板中提取类，提升开发效率。
head:
  - - meta
    - name: keywords
      content: UnoCSS, Pug, 提取器, 模板, CSS 生成
---

# Pug 提取器

支持从 Pug 模板中提取类。

## 安装

::: code-group

```bash [pnpm]
pnpm add -D @unocss/extractor-pug
```

```bash [yarn]
yarn add -D @unocss/extractor-pug
```

```bash [npm]
npm install -D @unocss/extractor-pug
```

:::

```ts [uno.config.ts]
import extractorPug from '@unocss/extractor-pug'
import { defineConfig } from 'unocss'

export default defineConfig({
  extractors: [extractorPug()]
})
```
