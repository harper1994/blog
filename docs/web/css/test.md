# css样式
## 一行文本超出显示省略号
```css
    width: 200px;
    height: 200px;
    overflow: hidden;
    text-overflow: ellipsis;
    white-space: nowrap;
```
## 二行文本超出显示省略号
```css
    width: 200px;
    height: 36px;
    overflow: hidden;
    text-overflow: ellipsis;
    line-clamp: 2;
    display: flex;
    box-orient: vertical;
```
### css Reset样式
```css
body,h1,h2,h3,h4,h5,h6,hr,p,blockquote,dl,dt,dd,ul,li,ol,pre,form,fieldset,
legend,button,input,textarea,th,td,article,aside,details,figcaption,figure,footer,
header,hgroup,menu,nav,section,div,span,p,i,a,img {
    margin: 0;
    padding: 0;
}
html,body  {
    height: 100%;
    width: 100%;
}
a {
    text-decoration: none；
    cursor: pointer
}
a:hover {
    text-decoration: underline;
    outline: none
}
i {
    font-style: normal;
}
a:focus {
    outline: 0;
}
img {
    border: 0;
    vertical-align: middle;
}
ul,ol,dl {
    list-style-type:none
}
.clearfix:after {
    content:"." ;
    display:block ;
    height:0 ;
    clear:both ;
    visibility:hidden ;
}
```
