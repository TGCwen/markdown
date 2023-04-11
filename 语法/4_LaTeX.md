## 初识

行内：`$ …… $`
行间:

```latex
$$
……
$$
```

`\,` 小间隙	`\ + 空格` 间隙	`\quad` 大间隙	`\qquad` 更大	`\\` 换行
`\bf` (bold face,粗体)
`\text`  `\rm(罗马体)` 直体



## 希腊字母表

<img src="https://wen-image.oss-cn-beijing.aliyuncs.com/image-20220813191435620.png" alt="image-20220813191435620" style="zoom:33%;" />

## 上下标

```latex
a^2,a_1 \\
x^{y+z},p_{ij},p_ij \\
x_i,x_{\text i} \\
\text{A B},\rm{A B} \\
\text A B,\rm A B \\
{\rm A} B \\
\text{e},\text{i}

\overbrace, \underbrace 分别在表达式上、下方给出一个水平的大括号
\overbrace{1+2+\cdots+n}^{n个} \qquad \underbrace{a+b+\cdots+z}_{26}
```


$$
a^2,a_1 \\
x^{y+z},p_{ij},p_ij \\
x_i,x_{\text i} \\
\text{A B},\rm{A B} \\
\text A B,\rm A B \\
{\rm A} B \\
\text{e},\text{i} \\

\overbrace{1+2+\cdots+n}^{n个} \qquad \underbrace{a+b+\cdots+z}_{26}
$$

## 分式和根式

`\frac (fraction,分数)`  `\dfrac (display-style)(放大作用)`
`\sqrt (square root,平方根)`

```latex
\frac {1}{2}  \frac 1 3 \\
\frac 1 {x+y} \\
\frac {\frac 1 x + 1} {y + 1},
\frac {\dfrac 1 x + 1} {y + 1} \\
\sqrt 2 , \sqrt {x+y} , \sqrt [3]x
```


$$
\frac {1}{2}  \frac 1 3 \\
\frac 1 {x+y} \\
\frac {\frac 1 x + 1} {y + 1},
\frac {\dfrac 1 x + 1} {y + 1} \\
\sqrt 2 , \sqrt {x+y} , \sqrt [3]x
$$

##  普通运算符

```latex
\times (乘)	\cdot (center dot,中心点\点乘)	\div (divide,除)
\pm (plus-minus,±)	\mp (minus-plus,∓)
\ge (greater than or equal,大于等于)
\le (less than or equal,小于等于)
\gg (远大于)	\ll (远小于)
\ne (not equal,不等于)
\approx (approximate,约等于)
\equiv (equivalent,恒等于)
\cap (交集,帽子形状)	\cup (并集,杯子形状)
\in (属于)	\notin (不属于)	
\because (因为)	\therefore (所以)
\mathbb + 字母(blackboard bold,双影) 或者 \ + 大写字母 (仅限数集字母)
\mathcal (calligraphy,书法)	\mathscr (script,手迹)
\cdots (点乘S)	\vdots (vertical,垂直的)	\ddots (diagonal,对角的)
\infty (infinity,无穷) \part (partial,偏(微分))
```

> sin log lg lim max 等函数直接写实斜体的.
> 前面加上 \ 后者 \text 变成直体.
>
> lim 等角标可能会在右边
> \limits 强制变在下边

$$
+- \\
\times,\cdot,\div \\ 
\pm,\mp,\ge,\le \\
>,<,\gg,\ll,\ne,\approx,\equiv \\
\cap,\cup,\in,\notin,\subseteq,\subseteqq,\subsetneq,\subsetneqq \\
\varnothing,\forall,\exists,\nexists \\
\because,\therefore \\
\mathbb R,\R \Q \N \Z_+ \\
\mathcal F , \mathscr F \\
\cdots,\vdots,\ddots \\
\infty\ \part \\
$$

## 大型运算符

```latex
\sum (求和)	\prod (product,求积)	
\int (integral,积分)	\iint(重积分,以此类推)
\oint (回路积分)	\oiint (双重回积分)
```

$$
\sum,\prod \\
\int,\iint,\oint,\oiint \\
\sum_{i=0}^N \\
\frac{\sum_{i=1}^N x_i}{\prod_{i=1}^N x_i},
\frac{\sum\limits_{i=1}^N x_i}{\prod\limits_{i=1}^N x_i} \\
\int_{-\infty}^0 f(x)\,\text d x
$$

## 标注符号

```latex
\vec (vector,向量)单个字符	\overrightarrow (大箭头)
\bar (平均值)单个字符	\overline (多字符)
```

$$
\vec {a}\ \overrightarrow {AB} \\
\bar a \ \overline {AB} \\
\widepare {AAA}
$$

![image-20220814215218552](https://wen-image.oss-cn-beijing.aliyuncs.com/image-20220814215218552.png)

## 箭头

```latex
 \leftarrow (左箭头)
```

$$
\leftarrow,\Rightarrow,\Leftrightarrow,\longleftarrow
$$

<img src="https://wen-image.oss-cn-beijing.aliyuncs.com/image-20220815010700711.png" alt="image-20220815010700711" style="zoom: 67%;" />

## 括号&定界符

```latex
\lceil (左侧上取整)	\rceil (右)
\lfloor (左侧下取整)	\rfloor (右)

范围确定的话,在对应括号前加\left,\right, 括号可以自适应大小
如果只有单个括号,可以用在没有括号的 \left,\right 后加 . (虚空括号)

也可以在需要自适应的位置加 \bigg
```


$$
() \quad [] \quad || \quad \{\} \\
\lceil\ \rceil \\
\lfloor\ \rfloor \\

(0,\frac a 1]
\left(0,\frac a 1\right] \\

\frac {\part x} {\part y} | _{x=0} \ 
\left.\frac {\part x} {\part y} \right| _{x=0} \ 
\frac {\part x} {\part y} \bigg| _{x=0}
$$

## 多行公式

```latex
\begin{align}
……
\end{align}
默认左对齐,
可以在需要对齐的地方前加 & (ampersand)
```

$$
\begin{align}

a&=b+c+d \\
&=e+f

\end{align}
$$

## 大括号

```latex
f(x)=

\begin{cases}
……
\end{cases}
```

$$
f(x)=

\begin{cases}

\sin x, &-\pi \le x \le \pi \\
0,		&\text{其他}

\end{cases}
$$

## 矩阵

```latex
 {matrix}
{bmatrix} (bracket, 方括号)
{pmatrix} (parenthesis,圆括号)
{vmatrix} (vertical bar,竖向短线)
```

$$
\begin{matrix}

a & b & \cdots & c \\
\vdots & \vdots & \ddots & \vdots \\
e & f & \cdots & g 

\end{matrix}

\begin{bmatrix}

a & b & \cdots & c \\
\vdots & \vdots & \ddots & \vdots \\
e & f & \cdots & g 

\end{bmatrix}
$$

$$
\begin{pmatrix}

a & b & \cdots & c \\
\vdots & \vdots & \ddots & \vdots \\
e & f & \cdots & g 

\end{pmatrix}


\begin{vmatrix}

a & b & \cdots & c \\
\vdots & \vdots & \ddots & \vdots \\
e & f & \cdots & g 

\end{vmatrix}
$$

```latex
$$
f(x) = a + b \tag {1.1} 
$$
```

$$
f(x) = a + b \tag {1.1}
$$

 

> 参考：[LaTeX公式保姆级教程 (以及其中的各种细节)_哔哩哔哩_bilibili](https://www.bilibili.com/video/BV1no4y1U7At?spm_id_from=333.1007.top_right_bar_window_view_later.content.click&vd_source=f41e9df0ec627675553cb6f4a9a656b4)	[在线LaTeX公式编辑器-帮助文档 (latexlive.com)](https://www.latexlive.com/help#d65)	[LaTeX 公式篇 - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/110756681)

