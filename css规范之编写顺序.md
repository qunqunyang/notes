
### css编写样式规范 之属性编写顺序
代码一致性的原则

遵循先布局后内容的顺序
- 1）位置属性（position, top, right,z-index, display, float 等）
- 2)大小 (width , height, padding, margin)
- 3 ) 文字系列 (font, line-height, color, text-aligin)
- 4 ) 背景 (border, background)
- 5 ) 其他(动画,阴影…)

例如：

```
    .g-box {
        display: block;
        position:relative;
        top:10px;
        z-index:10;
        float: left;
        width: 500px;
        height: 200px;
        margin: 10px;
        padding: 10px;
        border: 10px solid;
        background: #aaa;
        color: #000;
        font: 14px/1.5 sans-serif;
    } 
```
> 而且可以看到posttion,top,z-index这几个属性是紧密连接在一起的，所以放在一块。


私有属性在前标准属性在后

```
    g-box {
        -webkit-box-shadow: 1px 1px 5px rgba(0, 0, 0, .5);
　　    -moz-box-shadow: 1px 1px 5px rgba(0, 0, 0, .5);
　　　  -o-box-shadow: 1px 1px 5px rgba(0, 0, 0, .5);
　　　  box-shadow: 1px 1px 5px rgba(0, 0, 0, .5);
    }
```

