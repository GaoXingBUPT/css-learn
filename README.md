# css-learn

## flex布局-换行属性(容器)

* flex-flow: row wrap;

  flex-flow: flex-direction flex-wrap 子元素沿着哪个方向流动，流动到终点是否允许换行

* flex-direction-子元素沿着哪个方向流动（主轴方向）

    > row 向右

    > column 向下

    > row-reverse 向左

    > column-reverse 向上
    
* flex-wrap-子元素流动到终点是否允许换行

    > nowrap 不换行（主轴尺寸超过了flex容器，做等比缩放）
    
    > wrap 换行
    
    > wrap-reverse 沿着交叉轴的反方向换行

## flex布局-align-items属性（容器）

 * align-items - 项目在交叉轴上如何对齐

    > flex-start - 交叉轴的起点对齐

    > flex-end - 交叉轴的终点对齐

    > center - 交叉轴中点对齐

    > baseline - 项目的第一行文字的基线对齐

    > strench - 如果项目未设置高度或设为auto，将占满整个容器的高度（！默认值）

## flex布局-flex属性（项目）

  * flex: 0 1 auto;

    > flex: flex-grow, flex-shrink, flex-basis；(后两个属性可选)

    > flex-grow 项目的放大比例，默认为0，即如果存在剩余空间，也不放大。

    > flex-shrink 项目的缩小比例，默认为1，即如果空间不足，该项目将缩小。

    > flex-basis 在分配多余空间之前，项目占据的主轴空间（main size）。浏览器根据这个属性，计算主轴是否有多余空间。它的默认值为auto，即项目的本来大小。(！设置不为auto时会覆盖项目本身的width/height)

## css3

  * 伪元素 ::after(:after) ::before(:before)

    > p:before 在每个 `<p>` 元素的内容之前插入内容。

    > 默认 inline

    > 这两个伪类下特有的属性content ，用于在 CSS 渲染中向元素逻辑上的头部或尾部添加内容。

    > 伪元素如果没有设置“content”属性，伪元素是无用的!!!可以设置content属性值为空，仅仅把他当做一个盒子。

  * transform

    > 对元素进行位移、旋转、缩放、倾斜操作，支持 2D 或者 3D 转换。

    > 是影响内部元素的，即一个元素设置了 transform 旋转、斜切等属性，其内部元素跟随变换。这时常常使用一个 absolute 定位的伪元素设置 transform 属性实现平行四边形、梯形、菱形等，不影响内部元素的效果。

  * transition

    > 元素从一种样式逐渐改变为另一种样式的效果

    > transition: 变换属性，变换时长，时间曲线(默认ease)，延迟(默认0)

  * animation

    > `@keyframes animationName {}`

    > animation: 动画名称，动画时常，动画时间曲线（默认ease），延迟（默认0），播放次数（默认1），动画方向（默认normal），是否暂停动画（默认running）

    > loading动画 `https://www.html5tricks.com/demo/css3-loading-cool-styles/index.html`

  * box-shadow

    > `box-shadow` 水平阴影的位置 垂直阴影的位置 阴影模糊半径 阴影扩散半径 阴影的颜色 阴影开始方向（默认是从里往外，设置inset就是从外往里）;

    > 当所给的阴影大于一个时，阴影在 z 轴应用的顺序为从前到后, 第一个指定的阴影在顶部.

    > inset 此时阴影会在边框之内 (即使是透明边框）、背景之上、内容之下。

  * border

    > `border-image` 图片url 图像边界向内偏移 图像边界的宽度(默认为边框的宽度) 用于指定在边框外部绘制偏移的量（默认0） 铺满方式--重复（repeat）、拉伸（stretch）或铺满（round）（默认：拉伸（stretch））

      * `border-image-outset` 属性定义边框图像可超出边框盒的大小。

      * `border-image-repeat` 定义图片如何填充边框。或为单个值，设置所有的边框；或为两个值，分别设置水平与垂直的边框。

      * `border-image-slice` 属性会将图片分割为9个区域：四个角，四个边（edges）以及中心区域。四条切片线，从它们各自的侧面设置给定距离，控制区域的大小。

      * `border-image-source` 用于声明元素的边框图片（border-image）的资源。

      * `border-image-width` 定义图像边框宽度。假如border-image-width大于已指定的border-width，那么它将向内部(padding/content)扩展。

    > `border-radius`

      * `border-radius: n1,n2,n3,n4;` n1-n4四个值的顺序是：左上角，右上角，右下角，左下角。

  * background

    > background-clip 制定背景绘制（显示）区域

    > background-origin 指定background-position属性应该是相对位置

      * border-box

      * padding-box

      * content-box

    > background-size

      * contain

      * cover 

      * auto 100%

      * 400px 
    
    > background-position 为每一个背景图片设置初始位置。 这个位置是相对于由 background-origin 定义的位置图层的

      * 百分比 `(container width - image width) * (position x%) = (x offset value)``(container height - image height) * (position y%) = (y offset value)`

  * 文字：换行、超出省略

  * 渐变
  * 颜色
  * 滤镜

  * 媒体查询
  * 盒模型

  * 布局：弹性布局、多列布局、栅格布局