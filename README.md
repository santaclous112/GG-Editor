[English](README.en-US.md) | 简体中文

<h1 align="center">GGEditor</h1>

<div align="center">

基于 [G6](https://github.com/antvis/g6) 和 [React](https://github.com/facebook/react) 的可视化图编辑器

[![GitHub](https://img.shields.io/github/license/alibaba/GGEditor)](LICENSE)
[![npm](https://img.shields.io/npm/v/gg-editor)](https://www.npmjs.com/package/gg-editor)
[![npm](https://img.shields.io/npm/dm/gg-editor)](https://www.npmjs.com/package/gg-editor)

</div>

## 安装

### npm

```sh
npm install --save gg-editor
```

### umd

```html
<script src="https://unpkg.com/gg-editor@${version}/dist/index.js"></script>
```

## 使用

### 流程图

```jsx
import GGEditor, { Flow } from 'gg-editor';

const data = {
  nodes: [
    {
      id: '0',
      label: 'Node',
      x: 55,
      y: 55,
    },
    {
      id: '1',
      label: 'Node',
      x: 55,
      y: 255,
    },
  ],
  edges: [
    {
      label: 'Label',
      source: '0',
      target: '1',
    },
  ],
};

<GGEditor>
  <Flow data={data} />
</GGEditor>;
```

### 脑图

```jsx
import GGEditor, { Mind } from 'gg-editor';

const data = {
  label: 'Central Topic',
  children: [
    {
      label: 'Main Topic 1',
    },
    {
      label: 'Main Topic 2',
    },
    {
      label: 'Main Topic 3',
    },
  ],
};

<GGEditor>
  <Mind data={data} />
</GGEditor>;
```

## 文档

- [API 文档](https://www.yuque.com/ggeditor/api)

## 示例

```sh
# 克隆仓库
$ git clone https://github.com/gaoli/GGEditor.git

# 切换目录
$ cd gg-editor

# 安装依赖
$ npm install

# 运行示例
$ npm start
```

| 类型 | 示例                                            |
| ---- | ----------------------------------------------- |
| 图表 | [Flow](examples/flow)                           |
| 图表 | [Mind](examples/mind)                           |
| 组件 | [Command](examples/component-command)           |
| 组件 | [ItemPanel](examples/component-item-panel)      |
| 组件 | [DetailPanel](examples/component-detail-panel)  |
| 插件 | [EditableLabel](examples/plugin-editable-label) |
| 插件 | [ItemPopover](examples/plugin-item-popover)     |
| 插件 | [ContextMenu](examples/plugin-context-menu)     |
