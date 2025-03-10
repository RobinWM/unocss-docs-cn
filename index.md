---
layout: home
title: UnoCSS 中文文档 - 即时按需的原子级CSS引擎
description: 获取最新版本的UnoCSS中文文档，了解强大的定制化功能和快速的性能
head:
  - - meta
    - name: keywords
      content: UnoCSS, CSS引擎, 前端开发, 自定义样式
  - - link
    - rel: canonical
      href: https://unocss.net

hero:
  image:
    src: /logo.svg
    alt: UnoCSS
  name: 'UnoCSS'
  text: 即时按需的原子级CSS引擎
  tagline: 可定制的·强大的·快速的·快乐的
  actions:
    - theme: brand
      text: 入门
      link: /guide/
    - theme: alt
      text: 交互式文档
      link: https://unocss.dev/interactive/
      target: _blank
    - theme: alt
      text: 演练场
      link: https://unocss.dev/play/
      target: _blank

features:
  - icon: <span class="i-carbon:ibm-toolchain"></span>
    title: 完全可定制
    details: 无核心工具，所有功能都通过预设提供。
    link: /guide/
    linkText: 开始使用
  - icon: <span class="i-carbon-meter-alt"></span>
    title: 即时的
    details: 无解析、无抽象语法树、无扫描。它比 Windi CSS 或 Tailwind JIT 快5倍。
  - icon: <span class="i-carbon-wind-gusts"></span>
    title: 轻量级的
    details: '零依赖且适用于浏览器：~6kb min+brotli'
  - icon: <span class="i-carbon-ibm-cloud-transit-gateway"></span>
    title: 丰富的集成能力
    details: '对Vite、Webpack、PostCSS、CLI、VS Code、ESLint等工具的一流支持'
    link: /integrations/vite
    linkText: '了解更多'
  - icon: <span class="i-carbon-asset"></span>
    title: 快捷方式
    details: '通过别名或动态分组实现工具类'
    link: /config/shortcuts
    linkText: '配置和使用'
  - icon: <span class="i-carbon:code"></span>
    title: '属性化模式'
    details: '在属性中对工具类进行分组'
    link: /presets/attributify
    linkText: '@unocss/preset-attributify'
  - icon: <span class="i-carbon-face-wink hover:i-carbon-face-satisfied"></span>
    title: 纯 CSS 图标
    details: '将任何图标作为单个类使用'
    link: /presets/icons
    linkText: '@unocss/preset-icons'
  - icon: <span class="i-carbon:group-objects"></span>
    title: 变体组
    details: '使用常见前缀的组合工具类的速记方式'
    link: /transformers/variant-group
    linkText: '@unocss/transformer-variant-group'
  - icon: <span class="i-carbon:at"></span>
    title: CSS 指令
    details: '使用 @apply 指令在 CSS 中重用工具类'
    link: /transformers/directives
    linkText: '@unocss/transformer-directives'
  - icon: <span class="i-carbon-tree-view-alt scale-x--100"></span>
    title: 编译模式
    details: '在构建时将多个类合成为一个类'
    link: /transformers/compile-class
    linkText: '@unocss/transformer-compile-class'
  - icon: <span class="i-carbon:inspection"></span>
    title: 检查器
    details: '交互式检查和调试'
    link: /tools/inspector
    linkText: '@unocss/inspector'
  - icon: <span class="i-carbon:executable-program"></span>
    title: CDN 运行时构建
    details: '只需一行 CDN 引入即可使用 UnoCSS'
    link: /integrations/runtime
    linkText: '@unocss/runtime'
---
