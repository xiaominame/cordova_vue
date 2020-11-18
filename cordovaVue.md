<!--
 * @Author: your name
 * @Date: 2020-11-10 18:24:03
 * @LastEditTime: 2020-11-18 19:23:44
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
##### 三.cordova安装
npm

node


cordova

```

- cordova编译

```
cordova build

cordova run android

```
### vue3.0理论基础


var vm = new Vue({

    el:"@box",
    data:{
        myname:"hello",
        isShow:true,
        isCreated:true,
        isActive:true,
        dataList:[],
        classobj:{
            a:true,
            b:true,
            c:true
        }
    },
    methods:{
        handClick(){

        }
    }

})

- 事情，点击

@click = "handClick()" <br>
或者 <br>
v-on:click="handClick()" 

- 创建和删除
```
v-show = "isShow"

v-if = "isCreated"

v-bind:class = "isActive ? 'red':'yellow' <br>
或者 <br>
:class="isActive ? 'red':'yellow' <br>

input : @input @change
```
- 双向绑定的指令

```
v-model

<input type="text" v-model="myname">
```
- 循环现实

```
v-for
<ul>
<li v-for="(data,index) in dataList>
{{data}}
</li>
</ul>

this.dataList.push(data);

数组的删除
this.dataList.splice(0,1)
```

- 解析html
```
v-html

<div v-html="myhtml"></div>
```

- class与style
```
多个class是面对对象

v-if

v-else-if

v-else

```

- 列表渲染

```
template 用于条件渲染 
<template v-if="isCreate">

</template>

数组对象
data
<li v-for="(data,index) in dataList" :key= data.id>
{{data}}
</li>
理想的key值是每项都有的且唯一的id。data.id
```

- 模糊查询
```
数组
filter
```