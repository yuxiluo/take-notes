#### 什么是BFC 
> BFC(Block Formatting Context) - 直译为"块格式化上下文". 一个独立的块级渲染区域

#### 创建BFC的常用方式
- overflow不为visible
- float属性不为name
- position为absolute或fixed
- display为inline-block、table-cell、table-caption、flex、inline-flex
- 注: display: table也认为可以生成BFC, 主要原因是table会默认生成一个匿名的table-cell, 正是这个匿名的table-cell生成了BFC

#### 解决问题
- 阻止外边距叠加
- 阻止围绕浮动元素
- 子元素浮动导致父容器高度塌陷(也可以通过清除浮动来解决)

#### BFC的约束规则
- 内部的Box绘制垂直方向, 一个接一个地放置
- Box垂直方向的距离由margin决定,属于同一个BFC的两个相邻的Box的margin会发生重叠
- BFC的区域不会与float box重叠
- 计算BFC的高度时, 浮动元素也参与计算



































