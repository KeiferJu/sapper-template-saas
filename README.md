# 介绍
sapper的webpack模板，在官方基础上集成了saas的编译。

使用：
```
<style src="./style.scss"></style>

<!-- Or -->

<style lang="scss">
  $color: red;

  .test{
    color: $color;
  }
</style>

<!-- Or -->

<style lang="scss">
 @import "./style.scss";
</style>
```

还在里面加入了一个简单的事件总线。
```
/**
 * 事件总线
 *
 * 使用方法:
 *  1. 引入组件类
 *         import EventBus from '../service/EventBus'
 *  2. 事件输出与订阅
 *         输出：EventBus.emit('ww.myevent','nihao1')
 *
 *         订阅：EventBus.addEventListener('ww.myevent', (data) => {
 *              name = data;
 *	       })
 *
 */
 ```