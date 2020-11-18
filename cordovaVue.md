<!--
 * @Author: your name
 * @Date: 2020-11-10 18:24:03
 * @LastEditTime: 2020-11-10 18:26:49
 * @LastEditors: Please set LastEditors
 * @Description: In User Settings Edit
 * @FilePath: /cordova_vue/Users/xiaomi/grt/doc/web/vue/cordova_vue/cordovaVue.md
-->
##### 一.创建vuejs项目

- 前提条件:已经安装node可以正常使用npm命令并且全局安装vue-cli工具
```
  npm install vue-cli -g
```

- 使用vue初始化基于webpack的新项目
```
  vue init webpack my-project
```
- 项目创建完成后，安装基础模块
```
  cd myproject;
  npm install;
```
- 安装完成后之后可以在开发模式下运行项目并预览项目效果
```
  npm run dev;
```
- 如果项目可以正常启动，即可继续安装vue的辅助工具
```
  npm install vue-router --save (路由管理模块)
  npm install vuex --save (状态管理模块)
  npm install vue-resource --save (网络请求模块)
```

##### 二.framework7-vue + cordova 构建app

环境:nodejs、android sdk

安装:
```
npm install -g cordova

npm i framework7-cli cordova -g

npm install -g ionic
```

1.创建项目
```
framework7 create myApp
```

2.添加cordova的组件(plugin)

```
framework7 cordova plugin add cordova-plugin-media
```