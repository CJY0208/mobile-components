# Mobile Components（源码暂不开放）

移动端组件库

## 安装

```bash
yarn add @cjy0208/mobile-components
# 或者
npm install @cjy0208/mobile-components --save
```

## 按需加载

配合 [babel-plugin-import](https://github.com/ant-design/babel-plugin-import) 实现按需加载

```js
// babel.config.js
module.exports = {
  plugins: [
    [
      'babel-plugin-import',
      {
        libraryName: '@cjy0208/mobile-components',
        libraryDirectory: 'lib/exports', // or 'es/exports'
        camel2DashComponentName: false,
        style: (name) => `${name}/style.less`, // or `${name}/style.css`
      },
      '@cjy0208/mobile-components',
    ],
  ],
}
```
