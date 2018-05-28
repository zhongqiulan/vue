# Jackblog Vue 版
[![Dependency Status](https://david-dm.org/jackhutu/jackblog-vue.svg)](https://david-dm.org/jackhutu/jackblog-vue) 
[![devDependency Status](https://david-dm.org/jackhutu/jackblog-vue/dev-status.svg)](https://david-dm.org/jackhutu/jackblog-vue#info=devDependencies)  

Jackblog 是使用 Node.js + MongoDB + 其它客户端框架开发的个人博客系统,前后端分离,仿简书模板.    
服务端有: [express 版](https://github.com/jackhutu/jackblog-api-express) , [koa 版](https://github.com/jackhutu/jackblog-api-koa)         
客户端有: [angular1.x 版](https://github.com/jackhutu/jackblog-angular1) , [angular2.x 版](https://github.com/jackhutu/jackblog-angular2) , [react 版](https://github.com/jackhutu/jackblog-react) , [vue 版](https://github.com/jackhutu/jackblog-vue)    
移动端有: [react native 版](https://github.com/jackhutu/jackblog-react-native-redux), [ionic2.0 版](https://github.com/jackhutu/jackblog-ionic2)      
##### 此为客户端vue版, 需要配合服务端使用. 

> 服务端任选一种, 请预先安装并启动服务端

## 开发

```
$ git clone git@github.com:jackhutu/jackblog-vue.git
$ cd jackblog-vue
$ npm install
$ npm run dev
```
在浏览器中自动打开 http://localhost:3000

## 调试
- 默认开启 vue-devtools [chrome浏览器扩展](https://github.com/vuejs/vue-devtools), 生产环境自动关闭

### 目录结构

```
.
├── README.md           
├── dist                     // 项目build目录
├── logs                     // 生产环境日志目录
├── src                      // 生产目录
│   ├── api                  // API 请求
│   ├── assets               // css 和图片资源
│   ├── components           // 组件
│   ├── utils                // 工具函数
│   └── store            		 // vuex相关文件, store,action
│   └── config.js            // api url, cookie domain等配置文件
│   └── index.html           // 主页html
│   └── routes.js            // 路由配置
│   └── index.js             // 入口文件
├── .babelrc                 // babel配置
├── .eslintrc.json           // eslint配置
├── History.md               // 更新日志
├── process.json             // pm2配置文件
├── server.js                // 生产环境启动server
├── webpack.config.js        // Webpack 配置文件
```

## 生产环境构建  
 
```
$ npm run build
```

## 线上布署
```
$ pm2 start process.json
```

## License
MIT