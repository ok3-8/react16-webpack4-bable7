# (React16,Webpack4, Babel7) => (<App />)（2019）

> React16.x+Webpack4.x+Babel7.x 搭建基础骨架

## 项目初始化

通过`npm init -y`初始化项目，生成package.json文件

## 在本地安装 webpack4，安装 webpack-cli

```
npm install webpack webpack-cli --save-dev
```

装webpack4各种常用加载器、插件和工具

```
npm i clean-webpack-plugin html-webpack-plugin --save-dev
npm i webpack-dev-server webpack-merge --save-dev
npm i file-loader url-loader style-loader css-loader babel-loader --save-dev
```

## 在本地安装 babel7 和它一些核心的包

项目安装`@babel/core` `@babel/preset-env` `@babel/preset-react`，同时安装`@babel/polyfill`
```
npm i -D @babel/core @babel/preset-env @babel/preset-react
npm i -S @babel/polyfill
```

先来看一下主要的包，babel 7 对于包进行了一些简化。
- @babel/cli: 用于执行相应命令 
- @babel/core: 核心包，将 js 代码分析成 AST 
- @babel/preset-env: 包含 es6+ 的语法转换规则，如箭头函数、const 等 
- @babel/polyfill: es6 内置对象和函数的垫片，如 Promise、Array.from 等 
- @babel/plugin-transform-runtime: 防止 polyfill 污染全局变量 
- @babel/runtime: 与 @babel/plugin-transform-runtime 配套使用

## 安装 React16

```
npm i -S react react-dom react-router-dom
```

## 说明

其它配置看项目目录结构描述。

## 目录结构描述

├── README.md                   // README
├── docs                        // for github page
├── config                      // 配置
│   ├── webpack.base.conf       // 配置控制
│   ├── webpack.dev.conf        // 开发环境
│   └── webpack.prod.conf       // 生产环境
├── src                         // 应用入口
│   ├── assets                  
│   ├── components              
│   ├── style                   
│   ├── App.jsx                 
│   ├── index.html              
│   └── index.js                
├── package.json                // package.json 
└── .babelrc                    // babelrc




















