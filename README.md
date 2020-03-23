# 图形学学习
|方法|描述|
|:--|:--|
|fill()|填充路径|
|stroke()|描边|
|arc()|创建圆弧|
|rect()|创建矩形|
|fillRect()|绘制矩形路径区域|
|strokeRect()|绘制矩形路径描边|
|arcTo()|创建两切线之间的弧/曲线|
|beginPath()|起始一条路径，或者重置当前路径|
|moveTo()|把路径移动到画布中的指定点，不创建线条|
|lintTo()|添加一个新点，然后在画布中创建从该点到最后指定点的线条|
|closePath()|创建从当前点回到起始点的路径|
|clip()|从原始画布剪切任意形状和尺寸的区域|
|quadraticCurveTo()|创建二次方贝塞尔曲线|
|bezierCurveTo（）|创建三次方贝塞尔曲线|
|isPointInPath()|如果指定点位于当前路径中，则返回 true，否则返回 false|

line 的样式
|方法|描述|
|:--|:--|
|lineCap|设置或返回线条的结束断点样式|
|lineJoin|设置或返回两条线相交时，所创建的拐角类型|
|lineWidth|设置或返回当前的线条宽度|
|miterLimit|设置或返回最大斜接长度|

图形转换
|方法|描述|
|:--|:--|
|scale()|缩放当前绘图|
|rotate()|旋转当前绘图|
|translate()|重新映射画布上的（0， 0）位置|
|transform()|替换绘图的当前转换矩阵|
|setTransform|将当前转换重置为单位矩阵，然后运行transform()|

## 圆弧角度
* 右：0
* 下：0.5 * Math.PI
* 左：Math.PI
* 上：1.5 * Math.PI

## lineTo 和 moveTo 注意事项
* 如果没有 moveTo，那么第一次 lineTo 的就视为 moveTo
* 每次 lineTo 后如果没有 moveTo，那么下次 lineTo 的开始点为前一次 lineTo 的结束点。