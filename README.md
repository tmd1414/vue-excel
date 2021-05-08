# vexcel

> A Vue.js project

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
整体预览图
[!image](https://github.com/tmd1414/vue-easy-excel/blob/master/%E6%95%B4%E4%BD%93%E9%A2%84%E8%A7%88%E5%9B%BE.jpg)

```

For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).
参数配置
```
{
  showToolBar:true,
  showColHeader:true,
  showRowHeader:true,
   formats:[
    {
    
    name:""
    }
    ],
    fonts: ["宋体"],
    formulas:[],
    value: {
    rows:[
          {"height":22},
          {"height":22}
         ]
    cols:[
          {"width":100,"index":"A"}
         ]
    "1":{
      "1":{
        "text":"asdfasf",
        "rowspan":3,
        "colspan":4,
        "fontWeight":"bold",
        "font":"STFangsong",
        "fontStyle":"italic",
        "textDecoration":"underline",
        "color":"rgb(255, 0, 0)",
        "backgroundColor":"rgb(0, 0, 0)"
        },
       "2":{
        "text":"",
        "invisable":true,
        "merge":[1,1]
        }
    }
    }
}
```
