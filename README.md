![](示例.png)

# 炫丽的时钟效果

### 改编自[慕课网-炫丽的倒计时效果Canvas绘图与动画基础](http://www.imooc.com/learn/133)
* 使用了两个canvas来分别绘制时钟和跳动的小球;
* 在`drawNum()`函数中使用了闭包来封装私有变量idx，从而实现了局部重绘，并且减少了代码量。
```javascript
 function drawNum(){
      var _idx ;
      return function(ctx,idx,left,top){
          if(idx != _idx){
          ...
           _idx = idx;
          }
      };
  }
```

