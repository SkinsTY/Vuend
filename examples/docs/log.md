##### 介绍
###### 什么是vuend？
一个基于vue.js的UI框架，用于快速构建移动端应用（初出茅庐，小试牛刀）  
<a href="https://github.com/Tianyazz/Vuend">https://github.com/Tianyazz/Vuend</a>   
<br />
*****
<br />

#### 安装 Install
npm install vuend -D

<br />

#### 本项目采用了rem可伸缩布局方案 lib-flexible，所以得安装 lib-flexible
npm install lib-flexible -D

<br />

#### main.js导入使用css

``` javascriptimport Vue from 'vue'
import vuend from 'vuend'
import 'vuend/dist/vuend.min.css'
import 'lib-flexible'

Vue.use(vuend)
```
<br />

*****
<br />

#### 2018-10-12 更新1.0.1版本
##### vuend 组件
<br />

组件名称|组件标签|描述
---|:--:|---:
EndButton|`<end-button></end-button>`|按钮
EndRadio|`<end-radio></end-radio>`|单选框
EndLayout|`<end-row></end-row>`<br />`<end-col></end-col>`|flexbox弹性布局
EndInput|`<end-input></end-input>`|文本框
EndToggle|`<end-toggle></end-toggle>`|开关按钮
EndCheckbox|`<end-checkbox></end-checkbox>`|复选框
EndList|`<end-list></end-list>`|列表
EndSearch|`<end-search></end-search>`|搜索
EndTextarea|`<end-textarea></end-textarea>`|文本域
EndTabs|`<end-tabs></end-tabs>`|选项卡
EndSelect|`<end-select></end-select>`|选择列表
<br />

*****
<br />

##### vuend 服务
<br />

服务名称（全局变量）|描述
---|:--:|---:
$toast|文字提示
$dialog|对话框
$loading|加载提示
<br />

****
<br />

#### Thanks to
- [voinc](https://github.com/wangdahoo/vonic)
- [element](https://github.com/ElemeFE/element)
- [vue-ui-docs](https://github.com/kitorv/vue-ui-docs)

<style lang="scss" scoped>
@import '~global/global';
h5 {
  margin-bottom: $px10;
}
h6 {
  margin-bottom: $px10;
  font-size: $px24;
  font-weight: normal;
}
p {
  font-size: $px20;
}
code {
  background: $gray;
  padding: $px10 $px20;
  font-size: $px20;
}
table {
  width: 100%;
  thead {
    background: $gray;
  }
  th, td {
    padding: $px20;
    border: 1px solid #ccc;
    font-size: $px20;
    text-align: center !important;
    code {
      background: $gray;
      padding: px2rem(5px);
      @include radius;
      font-size: $px20;
    }
  }
  tr:nth-child(2n) {
    background: $gray;
  }
}
ul {
  padding-left: px2rem(50px);
  li {
    list-style: disc;
  }
}
</style>