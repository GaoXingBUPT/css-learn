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

  * 伪元素 ::after ::before

    > 这两个伪类下特有的属性content ，用于在 CSS 渲染中向元素逻辑上的头部或尾部添加内容。

    > 伪元素如果没有设置“content”属性，伪元素是无用的!!!可以设置content属性值为空，仅仅把他当做一个盒子。

  * transition

    > 元素从一种样式逐渐改变为另一种样式的效果

    > transition: 变换属性，变换时长，时间曲线(默认ease)，延迟(默认0)

  * animation

    > `@keyframes animationName {}`

    > animation: 动画名称，动画时常，动画时间曲线（默认ease），延迟（默认0），播放次数（默认1），动画方向（默认normal），是否暂停动画（默认running）

    > loading动画 `https://www.html5tricks.com/demo/css3-loading-cool-styles/index.html`