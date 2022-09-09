# Icoding-APP-Project-02

# 第三十课： Flex 弹性布局

- display: flex; 弹性布局， 元素自身以块级元素显示。
- display: inline-flex; 弹性布局，元素自身以行内块元素显示

> Flex 布局， 项目子元素的 float, clear & vertical-align 属性将失效。

- flex-basix: auto; 元素的宽为自动-inline-block.
- flex-wrap: nowrap; 子元素默认放不下的时候， 不会换行.

## Flex 容器属性

1. flex direction:

   - row / column

2. flex-wrap: nowrap; - default

   - nowrap / wrap / wrap-reverse

3. flex-flow: colum wrap; 复合写法；

4. justify-content: 项目在主轴上对齐方式 - flex-start; -default;

   - flex-start / flex-end / center / space-between / space-around / space-evenly

5. align-items: stretch; - 项目在交叉轴上对齐方式, `只对单行有效`；
   - stretch / flex-start / flex-end / center / baseline

令 flex 元素居中的方法:

> 水平居中: `justify-content: center;`  
> 垂直居中: `align-items: center;`

6. align-content: stretch; - 定义了多根轴线在交叉轴对齐方式 (多行)；

- stretch / flex-start / flex-end / center / space-between / space-around

<br>

## 三， Flex 项目属性

- order: 项目的排列顺序； 默认为 0， 数值约小排越前；

- align-self： 单个项目对齐方式；

- flex-grow: 当容器有剩余空间的时候才会生效；

  - felx-grow: 1; 当容器没设置宽度的时候， flex-grow=1 意思是元素会跟着父元素的宽度来 扩大；

- flex-shrink: 项目主轴上缩放
   - 当所有 flex 项目`宽度的和大于容器`的时候才会发生收缩。

- flex-basis: 分配剩余空间前， 项目占主轴空间大小 (main size)
   - 优先级大于 width；

- flex 项目放大，缩小， 空间占据
   - flex 属性是 flex-grow, flex-shrink 和 flex-basis的简写，默认值为 `0 1 auto`.
   - 2个快捷值:
      - `flex: auto;` 表示 `flex: 1 1 auto;`
      - `flex: none` 表示 `flex: 0 0 auto;`


### Flex 弹性布局作业 - 30 个 CSS/CSS3 真实项目案例布局

- 26, 27, 28
