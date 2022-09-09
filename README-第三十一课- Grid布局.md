# Grid 网格布局

- Grid 布局是将容器划分成 "行" 和 "列"， 产生单元格, 然后指定"项目所在"的单元格, 可以看作 二维布局.

## 二， Grid 容器属性

1.  grid-template-columns: 属性定义每一列的列宽
    grid-template-rows: 属性定义每一行的行高
    - 属性值的 3 个单位:

(1) 绝对长度单位 px - grid-template-rows: 100px 100px 100px; - grid-template-columns: 100px 100px 100px;

(2) 百分% 单位
(3) fr 关键字 (fraction)
(4) repeat 函数

    - grid-template-rows: repeat(3, 100px);
    - grid-template-columns: repeat(3, 100px);

(5) auto-fill 关键字自动填充 - grid-template-columns: repeat(auto-fill, 100px); - 列能放多少就放多少；

(6) minmax()函数产生一个长度范围， 表示长度就在这个范围之中接受 2 个参数分别为最小值和最大值； - minmax(100px, 1fr); 表示最小宽为 300px, 最大为 1fr

(7) auto 关键字 - 表示 列宽或者行高 由浏览器自己决定长度；

(8) 网格线的名称 - grid-template-rows: [a1] 100px [a2]; - grid-template-columns: [b1] 200px [b2] auto [b3] 200ox [b4];

<br>

2. row-gap, column-gap, pag 属性
   - 属性值单位为 绝对单位 px 或者 %百分比
   - `gap: 10px 20px;` 是 row-gap: 10px 与 column-gap： 20px; 的简写;

<br>

3. grid-template-areas 属性
   - 用于指定网格区域, 一个区域由单个或多个单元格组成。
   - 需要配合项目属性 `grid-area` 一起使用

ex: `grid-template-areas:`
`"a a b"`
`"a a d"`
`"c c c";`

> 如果某些区域不需要利用, 则使用点(.) 表示

            grid-template-areas:
                "a .  . g"
                "a . . f"
                "c . . c";

<br>

4. grid-auto-flow 属性

   - row / column / row dense / column dense

- row-dense : 先行后列， 并且可能填满，尽量不出现空格。

<br>

5. justify-items 属性 - 设置单元格内容的水平位置；

   - stretch / start / end / center

> place-item: center; -表示: align-item & justify-items

<br>

9. justify-content 属性 - 属性设置整个内容区域在容器里面的`水平位置`；

默认: justify-content: start; 对齐容器的左边框

start / end / center / stretch / space-around / space-between / space-evenly

<br>

10. align-content 属性设置整个内容区域在容器里面的`垂直位置`；

> place-content: -属性表示: align-content 属性和 & justify-content 属性的合并简写法。

## Grid 项目属性

项目的位置是可以指定的，指定方法是通过指定项目的四个边框的位置，分别定位在那根网格线。

- grid-column-start

- grid-column-end

- grid-row-start

- grid-row-end

### grid-column-start: 1; grid-column-end: 3;

> 等同于: grid-column : 1/3;

## Grid 作业：

案例 29， 30
