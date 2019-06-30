---
order: 10
title:
  zh-CN: 自定义字段名
  en-US: Custom Field Names
---

## zh-CN

自定义字段名。

## en-US

Custom field names.

```jsx
import { Cascader } from 'antd';

const options = [
  {
    code: 'zhejiang',
    name: '技能组01',
    items: [
      {
        code: 'hangzhou',
        name: '陈火城',
              },
    ],
  },
  {
    code: 'jiangsu',
    name: '技能组02',
    items: [
      {
        code: 'nanjing',
        name: '王掌柜',
      },
    ],
  },
];

function onChange(value) {
  console.log(value);
}

ReactDOM.render(
  <Cascader
    fieldNames={{ label: 'name', value: 'code', children: 'items' }}
    options={options}
    onChange={onChange}
    placeholder="Please select"
  />,
  mountNode,
);
```
