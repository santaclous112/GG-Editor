[English](README.en-US.md)

<h1 align="center">GG-Editor</h1>

<div align="center">

</div>


### npm

```bash
npm install gg-editor --save
```

### umd

```html
<script src="https://unpkg.com/gg-editor@${version}/dist/index.js"></script>
```


[![Edit GGEditor - Flow](https://codesandbox.io/static/img/play-codesandbox.svg)](https://codesandbox.io/s/ggeditor-flow-hq64m?fontsize=14&hidenavigation=1&theme=dark)

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
  <Flow style={{ width: 500, height: 500 }} data={data} />
</GGEditor>;
```

### 脑图

[![Edit GGEditor - Mind](https://codesandbox.io/static/img/play-codesandbox.svg)](https://codesandbox.io/s/ggeditor-mind-2262q?fontsize=14&hidenavigation=1&theme=dark)

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
  <Mind style={{ width: 500, height: 500 }} data={data} />
</GGEditor>;
```



```bash

$ git clone https://github.com/santaclous112/GGEditor.git


$ cd gg-editor


$ npm install


$ npm start
```

### Contacts


![Gmail](https://github.com/santaclous112/MonilP-Portfolio/blob/master/src/components/Icon/svg/mailto.svg)               
        santaclous112@gmail.com

![Skype](https://github.com/santaclous112/MonilP-Portfolio/blob/master/src/components/Icon/svg/skype.svg)               
        live:.cid.772f958a47f37977

![Telegram](https://github.com/santaclous112/MonilP-Portfolio/blob/master/src/components/Icon/svg/telegram.svg)               
        PeaceStar01
