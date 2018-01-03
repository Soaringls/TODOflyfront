#  vue2-echo

![image](https://img.shields.io/badge/vue-2.5.2-blue.svg)
![image](https://img.shields.io/badge/vue--router-3.0.1-blue.svg)
![image](https://img.shields.io/badge/vuex-3.0.1-blue.svg)
![image](https://img.shields.io/badge/muse--ui-2.1.0-blue.svg)
![image](https://img.shields.io/badge/license-MIT-blue.svg)

## 前言
这半年多一直用Vue写项目，感觉用的挺得心应手，所以准备分享一些经验和记录成果。我上网搜了Vue的练手项目和视频教程，目前大多数都是音乐、购物车，后台管理那方面，可能因为这方面需求比较多吧。考虑之后打算从容易 -> 中等 -> 困难， 3个复杂度和不同类型的项目，一步步地带领大家深入Vue。这3个阶段的项目将会涉及Vue的大部分知识，如果你都能掌握，那么你就可以随心所欲地使用Vue去写单页面应用了。

此开源系列全部都是线上实践，并不像一些视频教程里面能实现差不多样子且没有考虑细节、兼容和使用体验的问题。一般作为上线项目，都会遇到一些极其不可理喻的需求且存在着许多麻烦的细节。往往这些才是我们最烦的，网上很多也搜索不到，又要自己去分析、实践，才能运用到自己项目上，这里会浪费大量大量的时间，所以在项目里我会尽可能注释大量的提示去帮助大家解决这些问题：都是我在线上项目实践过的一些经验，供大家参考。

## 技术栈
> [vue](https://cn.vuejs.org/v2/guide/)、[vue-router](https://router.vuejs.org/zh-cn/essentials/getting-started.html)、[vuex](https://vuex.vuejs.org/zh-cn/getting-started.html)、[axios（请求库）](https://github.com/axios/axios)、[muse-ui（移动端UI库）](http://www.muse-ui.org/#/install)

> [vue-awesome-swiper（轮播图）](https://github.com/surmon-china/vue-awesome-swiper)、[vue-progressbar（加载进度条）](https://github.com/hilongjw/vue-progressbar)、[lib-flexible（淘宝适配库）](https://github.com/amfe/lib-flexible)、[mockjs（数据模拟）](http://mockjs.com/)、[Material Icons（google图标）](http://google.github.io/material-design-icons/)

> [ES6/7（JS语法）](https://github.com/lukehoban/es6features)、[Stylus（css预处理器）](https://github.com/stylus/stylus)、[ESlint（JS风格规范）](https://github.com/standard/standard/blob/master/docs/RULES-zhcn.md)、[webpack3（资源处理）](https://github.com/webpack/webpack)

## 说明
> 开发环境 macOS 10.12.6、Chrome 61、 nodejs 8.4.0

> 如果对您有帮助，您可以点右上角 "Star"一下， 您的支持是我最大的动力！非常感谢！^_^ 🌹

> 或者您可以 "follow" 一下，我会不断开源更多的有趣实用的项目

> 如有问题请直接在 Issues 中提，或者您发现问题并有非常好的解决方案，欢迎 PR 👍

> 该项目是此开源系列的其中一个阶段，更多内容查看下方的最终目标

## 最终目标

- 第一阶段：echo回声（移动端，难度：简单 ~ 中等） —— [仓库地址](https://github.com/uncleLian/vue2-echo) —— [项目演示地址](http://echo.liansixin.win)

- 第二阶段：今日头条（移动端 & native，难度：困难） —— [仓库地址](https://github.com/uncleLian/vue2-news) —— [移动端演示地址](http://toutiao.liansixin.win)， [native端演示地址](http://native.liansixin.win)

- 第三阶段：头条号（pc端，难度：中等 ~ 困难） —— [仓库地址](https://github.com/uncleLian/vue2-health) —— 还在开发，敬请期待！（已实现核心功能）

##### 注：此系列只关注前端项目的实现，后端等知识不是此系列的范围，但会告知一二。

## 注意

> 1、因为vue-router使用 history 模式并且该项目没有后端支持，所以线上项目刷新之后是会出现404的，这里是需要后端配置一下的。在开发环境下不会出现这种问题，建议下载项目运行查看最佳效果。具体解释在router里面或者查看 [vue-router官网的解释](https://router.vuejs.org/zh-cn/essentials/history-mode.html)

> 2、该项目是纯前端项目，数据是使用mock模拟的，数据结构跟官方保持一致，只是没有了一些其他功能的数据，类似评论等。

> 3、手机查看项目有些浏览器不支持自动播放音乐的，需要手动触发。

## 效果演示 

[查看deme请戳这里](http://echo.liansixin.win)（请使用chrome手机模式预览）

### 移动端扫描下方二维码

<img src="https://github.com/uncleLian/vue2-echo/raw/master/screenshots/echo_QRcode.png" width="250" height="250"/>

## 功能

- [x] 全站内播放（单页面优点）
- [x] 播放 & 暂停 & 下一首
- [x] 播放模式： 默认、随机播放、单曲循环、列表循环
- [x] 播放进度条 & 可调节播放进度
- [x] 播放列表 & 可删除播放列表 & 可点击切换音乐
- [x] 一键播放
- [ ] 弹幕 （太耗移动web性能和个人时间，暂不实现啦）
- [ ] 手机铃声（好像只有app获取用户手机权限才能实现，web暂不可能实现，如果可以实现请告知我）

## 项目截图

<img src="https://github.com/uncleLian/vue2-echo/raw/master/screenshots/echo_index.png" width="365" height="619"/> <img src="https://github.com/uncleLian/vue2-echo/raw/master/screenshots/echo_index.gif" width="365" height="619"/>

<img src="https://github.com/uncleLian/vue2-echo/raw/master/screenshots/echo_detail.png" width="365" height="619"/> <img src="https://github.com/uncleLian/vue2-echo/raw/master/screenshots/echo_detail.gif" width="365" height="619"/>

<img src="https://github.com/uncleLian/vue2-echo/raw/master/screenshots/echo_fn.png" width="365" height="619"/> <img src="https://github.com/uncleLian/vue2-echo/raw/master/screenshots/echo_fn.gif" width="365" height="619"/>

## 目录结构

``` bash
├── build                        // 构建相关  
├── config                       // 配置相关
├── src                          // 源代码
│   ├── assets                   // 样式、图标等静态资源
│   ├── components               // 全局公用组件
│   |   ├── banner.vue           // banner组件
│   |   ├── error.vue            // 错误组件
│   |   ├── list.vue             // 列表组件
│   |   ├── loading.vue          // 加载组件
│   |   ├── musicBar.vue         // 音乐条组件
│   |   ├── sheet.vue            // 模态框组件
│   ├── config                   // 全局公用方法
│   |   ├── cache.js             // 缓存方法
│   |   ├── fetch.js             // 请求方法
│   |   ├── util.js              //  工具方法
│   ├── mock                     // mock数据
│   ├── page                   
│   |   ├── detail               //  详情页
│   |   ├── index                //  首页
│   ├── router                   // 路由
│   ├── store                    // 状态管理
│   ├── App.vue                  // 入口页面
│   └── main.js                  // 入口 加载组件 初始化等
├── static                       // 空文件夹，只作为github保留
├── .babelrc                     // babel-loader 配置
├── eslintrc.js                  // eslint 配置项
├── .gitignore                   // git 忽略项
├── index.html                   // html模板
└── package.json                 // package.json
```

## 安装运行

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8088
npm run dev

# build for production with minification
npm run build

本项目没有依赖JQuery，如需要使用JQuery，打开build目录的webpack.dev.conf.js 和 webpack.prod.conf.js 里面的JQuery代码，并npm install jquery -save
```

## 交流

欢迎热爱学习、忠于分享的朋友一起来交流
- QQ：771674109
- WX：L771674109
- Vue交流群：338241465 —— 广州-小鑫

## License

[MIT](http://opensource.org/licenses/MIT)

Copyright (c) 2017-present，uncleLian
