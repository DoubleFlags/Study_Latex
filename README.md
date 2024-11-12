[TOC]
# Study_Latex
学习Latex

# 希腊字母
$$
% \begin{align}
\delta,\alpha,\lambda\\
\Delta,\Lambda\\
\Alpha,\Beta\\
\phi,\Phi,\varphi\\
\epsilon,\varepsilon\\
\pi,\pi\\
% \end{align}
$$
![图片alt](res\png\image.png "图片title")
___

# 上下标
> ^上标，_下标，超过一个字符要用{}
> 
$$
a^2,a_1\\
a^{x+y},p_{ij},p_ij\\
$$
> 斜体表示变量,\rm和\text{} 直立体(罗马体)，其中\text{}支持空格显示
> 
> \mathrm 括号中文本转为直立体，\rm之后的文本都转为直立体
> 
$$
x_i,x_{\text i}\\
\text{A B},\rm{A B}\\
$$
> 不加括号则只对第一个字符生效
> 
$$
\text A B,\mathrm A B\\
{\rm A} B\\
$$
> 自然对数,虚数i,j为常量应该用直立体
> 
$$
\text{e},\text{i}
$$
___
# 分式与根式
> \frac(fraction,分数)
> 
$$
\frac{1}{2},\frac 1 2\\
\frac{1}{x+y}\\
\frac{\frac 1 x+1}{y+1},\frac{\dfrac 1 x+1}{y+1}
$$
> \sqrt(square root,平方根)
>
$$
\sqrt 2,\sqrt{x+y},\sqrt[3]{x}
$$

# 普通运算符
$$
+-\\
\times,\cdot,\div\\
$$
> (plus-minus),(minus-plus)
>
$$
\pm,\mp
$$
> (greater than or equal,大于等于),(less than or equal,小于等于),(approximate,约等于),(equivalent,恒等)
> 
$$
>,<,\ge,\le,\gg,\ll,\ne,\approx,\equiv\\
\cap,\cup,\in,\notin,\subseteq,\subsetneqq,\varnothing\\
\forall,\exists,\nexists\\
\because,\therefore\\
\mathbb R,\R,\N,\Z_+\\
\mathcal{F}\\
\cdots,\vdots,\ddots\\
\infty,\partial,\nabla,\propto,\degree\\
\sin x,\sec x\\
\log_2 x,\ln x,\lg x\\
\lim_{x \to 0} \frac {x} {\sin x}
$$
> 部分编辑器x->0可能显示在角标的位置，可以这么写
> 
$$
\lim\limits_{x \to 0} \frac {x} {\sin x}\\
\max x
$$
> 从上面可以看出运算符名称如果超过一个字符要用直立体
> 
___
# 大型运算符
>(product,乘积)
>
$$
\sum,\prod\\
\sum_i,\sum_{i=0}^N\\
\frac{\sum_{i=0}^N x_i}{\prod_{i=1}^N x_i},
\frac{\sum\limits_{i=0}^N x_i}{\prod\limits_{i=1}^N x_i}\\
\int,\iint,\iiint,\oint,\oiint\\
$$
> 写积分时，按标准写法，d为直立体，d前有一个小间隔使用\\,
> 
$$
\int_{-\infty}^0 f(x)\,\text{d}x
$$
> 关于空格，以下写法的间隔不一样
> 
$$
a\,a\\
a\ a\\
a\quad a\\
a\qquad a\\
$$
___
# 标注符号
>\vec只支持比较小的箭头,2个或更多字符的向量用\overrightarrow
>
$$
\vec x,\overrightarrow{AB}\\
\bar x,\overline{x}
$$
![图片alt](res\png\image2.png "图片title")
$$
\leftarrow,\rightarrow,\Rightarrow,\Leftrightarrow
$$
![图片alt](res\png\image3.png "图片title")
___
# 括号与定界符
$$
(),[],\{\}\\
\lceil,\rceil,\lfloor,\rfloor,||\\
$$
> 高度自适应，左右括号前加\left和\right
> 
$$
(0,\frac 1 a],\left(0,\frac 1 a\right]
$$
> 没有括号想高度自适应，加入虚拟括号\left.和\right.
> 
$$
\frac {\partial f} {\partial x}|_{x=0},
\left.\frac {\partial f} {\partial x}\right|_{x=0}
$$
___
# 多行公式
> \\\\是不规范的写法，不是全部的编辑器支持，规范的是用align环境
>
> 可以用&(ampersand)对齐
> 
$$
\begin{align}
a&=b+c+d\\
&=e+f
\end{align}
$$
___
# 大括号
$$
f(x)=
\begin{cases}
    
\sin x,&-\pi\le x \le pi\\
0,&其他


\end{cases}
$$
___
# 矩阵
> (bracket,方括号),(parenthesis,圆括号),(verticacl bar,横向竖线)
> 
$$
\begin{matrix}
    
a & b & \cdots & c\\
\vdots & \vdots & \ddots & \vdots\\
e & f & \cdots & g
\end{matrix}
\\
\begin{bmatrix}    
a & b & \cdots & c\\
\vdots & \vdots & \ddots & \vdots\\
e & f & \cdots & g
\end{bmatrix}

\begin{pmatrix}    
a & b & \cdots & c\\
\vdots & \vdots & \ddots & \vdots\\
e & f & \cdots & g
\end{pmatrix}

\begin{vmatrix}    
a & b & \cdots & c\\
\vdots & \vdots & \ddots & \vdots\\
e & f & \cdots & g
\end{vmatrix}
$$
> 矩阵符号用加粗直立体表示
> 
$$
\bf A,\bf B^{\rm T}
$$