# 技术栈

node
npm
vue
vue-router
stylus

# npm安装及配置

# webstorm配置

配置vue模板
`settings... --> Editor --> File and Code Templates`

如果是webstorm，它默认保存在临时文件，把settings=>appearance=>system=>synchornization=>最后一项勾去掉，热部署替换是没问题的

# webpack

# 制作图标字体

<https://icomoon.io>

# mock数据

json文件：`data.json`
`build/dev-server.js`中的`var apiRoutes = express.Router();`
chrome的`jsonview`插件

<http://rapapi.org/platform/home.do>

# reset.css

重置默认样式
<http://cssreset.com>

# eslint

`.eslintrc.js`
<http://eslint.org>
<http://eslint.org/docs/rules/semi>

# 组件拆分

flex布局

# vue-router

<https://router.vuejs.org/zh-cn/>
`npm install --save vue-router`

# 1像素bordre实现

`mixin.styl` border-1px
`base.styl` @media

# vue-resource

# css note

先写html结构，再写css

rgba 实现半透明
span inline-block 设置width与height才有用
position: relative 与 position: absolute
height 与 line-height
z-index
filter: blur(10px)  模糊效果

css sticky foot：如果页面内容不够长的时候，页脚粘贴在视窗底部；如果内容足够长时，页脚块会被内容向下推送
    fixed 布局的不足，内容过长时，页脚会覆盖页面内容
  套路：3层 `detail --> detail-wrapper clearfix --> detail-main`
            `detail --> detail-close`
  clearfix  清除浮动  base.styl
  
<http://caniuse.com>

# vue

star组件开发
vue 动画效果
transition='fade'
      transition: all 0.5s
      &.fade-transition
        opacity: 1
        background: rgba(7, 17, 27, 0.8)
      &.fade-enter,&.fade-leave
        opacity: 0
        background: rgba(7, 17, 27, 0)

$nextTick
// 改变数据时，vue是异步的，会放到一个更新队列里面
// 当下一个时间周期，nextTick觖发之后，dom才会更新
        
vue动画
子组与父组件之间的事件传递
动态获取动画进入与退出的位置
bezier曲线 <cubic-bezier.com>
两个动画时间启动时，卡的解决

禁止事件冒泡
@click.stop.prevent

router切换
状态保留keep-alive，请求的数据也会保存，不会重新发起请求
实现原理，就是将组件状态，保存在内存里

# 经典flex布局

flex 布局 阮一峰
<http://www.ruanyifeng.com/blog/2015/07/flex-grammar.html?utm_source=tuicool>

# 滚动条

<https://github.com/ustbhuangyi/better-scroll>

左右联动：依赖右侧Y轴坐标

# vue与dom交互

v-el
let foodList = this.$els.foodsWrapper.getElementsByClassName('food-list-hook');

$nextTick dom渲染好之后

# js

本地存储
window.localStorage

解析URL参数urlParse

# express


# 链接

<https://github.com/vuejs/vue-router>
<https://github.com/ustbhuangyi/better-scroll>
<http://webpack.github.io>

stylus中文文档 <http://www.zhangxinxu.com/jq/stylus/>
es6入门学习 <http://es6.ruanyifeng.com/>
eslint规则 <http://eslint.org/docs/rules>

设备像素比 <http://www.zhangxinxu.com/wordpress/2012/08/window-devicepixelratio>
Flex布局 <http://www.ruanyifeng.com/blog/2015/07/flex-grammar.html?utm_source=tuicool>
贝塞尔曲线测试(购物车动画) <http://cubic-bezier.com/>
