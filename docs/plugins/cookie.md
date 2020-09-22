# 插件的使用
## vue 中使用 Cookie
1. npm i vue-cookie -D
2. 在main.js中引入cookie并注册
```javascript
import VueCookie from 'vue-cookie'
Vue.use(VueCookie)
```
3. 使用cookie
- 存储cookie(对象要用JSON.stringify转成字符串)
```javascript
this.$cookie.set('key',JSON.stringify({pwd: this.password, name: this.loginKey}))
```
- 获取cookie值(JSON.parse转成对象)
```javascript
JSON.parse(this.$cookie.get('key')).name
```
- 删除cookie值
```javascript
this.$cookie.delete('key')
```
::: tip 提示
cookie的第三个值是cookie的存储时间。-1代表是永久，默认关闭是清除
:::