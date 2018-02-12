# vue-webpack-demo
使用 vue，vue-router 和 webpack 进行打包的 demo

## nginx 配置示例
如果希望使用特定的子目录，如之前使用 www.domain.com/ 访问想要改为 www.domain.com/vue 访问，
则需要修改如下内容：
1. 修改 webapp/config/index.js 将 `assetsPublicPath` 改为 `/vue/`
2. 修改 webapp/src/router/index.js 在 `router` 定义中添加 `base: '/vue/'`