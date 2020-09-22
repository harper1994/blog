# Vant
## 全局loading的使用
```javascript
import Vue from 'vue'
import { Toast } from 'vant'
import 'vant/lib/index.css'
Vue.use(Toast)
```
在用到的地方调用就好了
```javascript
this.$toast.loading({
    mask: true, //蒙层
    duration: 0, // 持续展示 toast
    forbidClick: true, // 禁用背景点击
    loadingType: 'spinner', // 图标类型
    message: '加载中...'
})
```
关闭loading

```javascript
this.$toast.clear()
```