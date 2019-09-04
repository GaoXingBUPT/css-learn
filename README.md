# css-learn

## flex布局-换行属性

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
## flex布局-align-items属性
 * align-items - 项目在交叉轴上如何对齐
    > flex-start - 交叉轴的起点对齐
    > flex-end - 交叉轴的终点对齐
    > center - 交叉轴中点对齐
    > baseline - 项目的第一行文字的基线对齐
    > strench - 如果项目未设置高度或设为auto，将占满整个容器的高度（！默认值）


