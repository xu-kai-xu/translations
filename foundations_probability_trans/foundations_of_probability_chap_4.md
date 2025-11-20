
## 数学期望[^4.1]

### 抽象勒贝格（Lebesgue）积分

令 $x$ 为随机变量，$A$ 为 $\mathcal{E}$ 构成的集合。给定一个正的 $\lambda$，构造以下和式：
$$
\tag{1}
S_{\lambda} = \sum_{k = -\infin} ^{k = + \infin} k \lambda \mathrm{P}\{ k \lambda \le x < (k + 1) \lambda, \quad \xi \sub A \}
$$
如果对每一个 $\lambda$ ，这个级数都绝对收敛，则当 $\lambda \rightarrow 0$时，$S_{\lambda}$ 趋近于一个确定值，且这个确定值为一个积分：
$$
\tag{2}
\int_{\lambda} x \mathrm{P}(d E)
$$
在这一抽象形式下，积分的概念由 Fréchet[^4.2] 提出。它对概率理论是必不可少的（dispensable）。（后文中读者会发现，除去一个常数因子外，变量 $x$ 在假设 $A$ 下的条件数学期望的常规定义与积分 ($2$) 中的定义恰巧相同）。

此处简要介绍下形式 $(2)$ 中的积分的最重要的一些性质。读者会在任何一本关于实变量的习题册中找到它们的证明，尽管这些证明通常都是基于 $\mathrm{P}(A)$ 是空间 $R^n$ 上集合的勒贝格测度（Lebesgue measure）这一假设做出的。将这些证明推广到更广义情形的过程并不包含任何新的数学问题，大多数证明（与勒贝格测度前提相比）都是完全一样的。

I. 如果随机变量 $x$ 在 $A$ 上可积，则它在 $A$ 的每一个子集 $A'$ 上可积（$A' \sub \mathcal{E}$）。

II. 如果 $x$ 在 $A$ 上可积，且 $A$ 可以分解为 $\mathcal{E}$ 上的不超过可数个的不相交集合 $A_n$，则
$$
\int_A x \mathrm{P}(dE) = \sum_n \int_{A_n} x \mathrm{P}(dE)
$$
III. 如果 $x$ 可积，则 $|x|$ 也可积，并且在这种情况下
$$
|\int_A x \mathrm{P}(dE)| \le \int_A |x| \mathrm{P}(dE)
$$
IV. 如果对于每一个事件 $\xi$ ，都有 $0 \le y \le x$ 成立，则 $x$、$y$  也可积[^4.3] ，并且在这种情况下
$$
\int_A y \mathrm{P}(dE) \le \int_A x \mathrm{P}(dE) 
$$
V. 如果 $m \le x \le M$，其中 $m$ 和 $M$ 为两个常数，则
$$
m \mathrm{P}(A) \le \int_A x \mathrm{P}(dE)  \le M \mathrm{P}(A)
$$
VI. 如果 $x$ 和 $y$ 可积，且 $K$ 和 $L$ 为两个实常数，则 $Kx + Ly$ 也可积，并且在这种情况下
$$
\int_A (Kx + Ly) \mathrm{P}(dE) = K \int_A x \mathrm{P}(dE)  + L \int_A y \mathrm{P}(dE) 
$$
VII. 如果级数
$$
\sum _n \int_A |x_n| \mathrm{P}(dE)
$$
收敛，则级数
$$
\sum _n x_n = x
$$
在除使得 $\mathrm{P}(B) = 0$ 成立的集合 $B$之外， 在集合 $A$ 的任意一点处都收敛。如果在 $A - B$ 外的任意位置都令 $x = 0$，则有
$$
\int_A x \mathrm{P}(dE) = \sum _n \int_A x_n \mathrm{P}(dE)
$$
VIII. 如果 $x$ 和 $y$ 等价（即 $\mathrm{P}\{ x \ne y \} = 0$），则对于任意的 $A \sub \mathcal{E}$，都有
$$
\tag{3}
\int_A x \mathrm{P}(dE) = \int_A y \mathrm{P}(dE)
$$
IX. 如果对于任意的 $A \sub \mathcal{E}$ 等式 $(3)$ 都成立，则 $x$ 和 $y$ 等价。

根据前述的积分定义还可以得出以下通常勒贝格理论中没有的性质：

X. 令 $\mathrm{P}_1(A)$ 和 $\mathrm{P}_2(A)$ 为两个定义在相同 $\mathcal{E}$ 上的概率函数，$\mathrm{P}(A) = \mathrm{P}_1(A) + \mathrm{P}_2(A)$，并且 $x$ 对于 $\mathrm{P}_1(A)$ 和 $\mathrm{P}_2(A)$，在 $A$ 上是可积的，则有
$$
\int_A x \mathrm{P}(dE) = \int_A x \mathrm{P}_1(dE) + \int_A x \mathrm{P}_2(dE) 
$$
XI. 每一个有界随机变量都是可积的。



### 绝对数学期望/条件数学期望

令 $x$ 为一随机变量，则积分
$$
\mathrm{E}(x) = \int _E x \mathrm{P}(dE)
$$
称为变量 $x$ 的数学期望（mathematical expectation）。由性质 III、IV、V、VI、VII、VIII、XI，可得 

I. $|\mathrm{E}(x)| \le \mathrm{E}(|x|)$；

II. 如果 $0 \le y \le x$，则 $\mathrm{E}(y) \le \mathrm{E}(x)$；

III. $\inf (x) \le \mathrm{E}(x) \le \sup (x)$；

IV. $\mathrm{E}(Kx + Ly) = K \mathrm{E}(x) + L \mathrm{E}(y)$；

V. 如果级数 $\sum_n \mathrm{E}(|x_n|)$ 收敛，则 $\mathrm{E}(\sum_n x_n) = \sum_n \mathrm{E}(x_n)$；

VI. 如果 $x$ 和 $y$ 等价，则 $\mathrm{E}(x) = \mathrm{E}(y)$；

VII. 每个有界的随机变量都有数学期望。

由积分的定义可得
$$
\mathrm{E}(x) = \lim \sum^{k = + \infin} _{k = - \infin} k m \mathrm{P} \{ km \le x < (k + 1) m \} \\
= \lim \sum^{k = + \infin} _{k = - \infin} \{ F((k + 1)m) - F(km) \}
$$
第二行是 Stieltjes 积分[^*]的定义
$$
\tag{1}
\int ^{+\infin} _{- \infin} a dF^{(x)} (a) = \mathrm{E}(x)
$$
公式 $(1)$ 可以作为数学期望 $E(x)$ 的定义。

现在令 $u$ 为基本事件 $\xi$ 的函数，且 $x = x(u)$ 为 $u$ 的单值函数，则
$$
\mathrm{P} \{ km \le x < (k + 1)m \} = \mathrm{P}^{(u)} \{ km \le x(u) < (k + 1)m \}
$$
其中 $\mathrm{P}^{(u)} (A)$ 是变量 $u$ 的概率函数。由积分的定义可得
$$
\int _E x \mathrm{P}(dE) = \int _{E^{(u)}} x \mathrm{P}^{(u)} (d E^{(u)})
$$
因此
$$
\tag{2}
\mathrm{E} (x) = \int _{E^{(u)}} x(u) \mathrm{P}^{(u)} (d E^{(u)})
$$
其中 $E^{(u)}$ 表示所有 $u$ 的可能取值构成的集合。

特别地，当 $u$ 本身是个随机变量时，可得
$$
\tag{3}
\mathrm{E}(x) = \int _E x \mathrm{P}(dE) = \int _{R^1} x(u) \mathrm{P}^{(u)} (d R^1) = \int ^{+ \infin} _{- \infin} x(a) d F^{(u)} (a)
$$
当 $x(u)$ 连续时，公式 $(3)$ 的最后一项积分为常规的 Stieltjes 积分。此处有必要指出，即使数学期望 $\mathrm{E}(x)$ 不存在，但积分
$$
\int ^{+ \infin} _{- \infin} x(a) d F^{(u)} (a)
$$
是存在的。$\mathrm{E}(x)$ 存在的充要条件是，积分
$$
\int ^{+ \infin} _{- \infin} |x(a)| d F^{(u)} (a)
$$
是有限的[^4.4]。

如果 $u$ 是空间 $R^n$ 中的点 $(u_1, u_2, \dots, u_n)$，则由公式 $(2)$ 可得
$$
\tag{4}
\mathrm{E}(x) = \int \int \cdots \int _{R^n} x(u_1, u_2, \dots, u_n) \mathrm{P}^{(u_1, u_2, \dots, u_n)} (d R^n)
$$
前文已经证明过，条件概率 $\mathrm{P}_B (A)$ 具有所有概率函数的性质。对应的积分
$$
\tag{5}
\mathrm{E} _B (x) = \int _E x \mathrm{P} _B (dE)
$$
称为随机变量 $x$ 在事件 $B$ 下的条件数学期望。由于
$$
\mathrm{P} (\bar{B}) = 0 \\
\int _{\bar{B}} x \mathrm{P} _B (dE) = 0
$$
所以由公式 $(5)$ 可得
$$
\mathrm{E}_B (x) = \int _E x \mathrm{P} _B (dE) = \int _B x \mathrm{P} _B (dE) + \int _{\bar{B}} x \mathrm{P} _B (dE) = \int _B x \mathrm{P} _B (dE)
$$
已知当 $A \sub B$ 时有
$$
\mathrm{P}_B (A) = \frac{\mathrm{P} (AB)}{\mathrm{P} (B)} = \frac{\mathrm{P} (A)}{\mathrm{P} (B)}
$$
由此得
$$
\tag{6}
\mathrm{E} _B (x) = \frac{1}{\mathrm{P}(B)} \int _B x \mathrm{P} (dE)
$$

$$
\tag{7}
\int _B P(dE) = \mathrm{P} (B) \mathrm{E} _B (x)
$$

由公式 $(6)$ 和以下等式
$$
\int _{A+B} x \mathrm{P} (dE) = \int _{A} x \mathrm{P} (dE) + \int _{B} x \mathrm{P} (dE)
$$
最终可得
$$
\tag{9}
\mathrm{E} _{A+B} (x) = \frac{\mathrm{P} (A) \mathrm{E} _A (x) + \mathrm{P} (B) \mathrm{E} _B (x)}{\mathrm{P} (A + B)}
$$
特别地，有如下等式
$$
\tag{9}
\mathrm{E} (x) = \mathrm{P}(A) \mathrm{E} _A (x) + \mathrm{P} (\bar{A}) \mathrm{E} _{\bar{A}} (x)
$$





### 切比雪夫（Tchebycheff）不等式

$f(x)$ 为实数 $x$ 的非负函数。如果对于 $x \ge a$，恒有 $f(x) \ge b > 0$，则如果数学期望 $\mathrm{E}\{ f(x) \}$ 存在，则对于任意随机变量 $x$，有
$$
\tag{1}
\mathrm{P}(x\ge a) \le \frac{ \mathrm{E}\{ f(x) \}}{b}
$$
证明：
$$
\mathrm{E}\{ f(x) \} = \int_E f(x) \mathrm{P} (dE) \ge \int_{(x \ge a)} f(x)  \mathrm{P} (dE) \ge b \mathrm{P} (x\ge a)
$$
例如，对任意正数 $c$，
$$
\tag{2}
\mathrm{P} (x \ge a) \le \frac{\mathrm{E} (e^{cx})}{e^{ca}}
$$
现在令 $f(x)$ 为非负的偶函数，并且对于 $x > 0$，$f(x)$ 为非减函数。则对于任意随机变量 $x$ 和任意选择的 $a > 0$，以下不等式成立：
$$
\tag{3}
\mathrm{P} (|x| \ge a) \le \frac{\mathrm{E \{ f(x) \} }}{ f(a)}
$$
特别地，
$$
\tag{4}
\mathrm{P} (|x - \mathrm{E}(x)| \ge a) \le \frac{\mathrm{E} f \{ x - \mathrm{E}(x) \} }{f(a)}
$$
当 $f(x) = x^2$ 时此关系尤为重要，由公式 $(3)$ 和 $(4)$ 可得
$$
\tag{5}
\mathrm{P}(|x| \ge a) \le \frac{\mathrm{E}(x^2)}{a^2}
$$

$$
\tag{6}
\mathrm{P} (|x - \mathrm{E}(x)| \ge a) \le \frac{\mathrm{E} \{ x - \mathrm{E}(x) \}^2 }{a^2} = \frac{\sigma^2(x)}{a^2}
$$

其中
$$
\sigma ^2(x) = \mathrm{E} \{ x - E(x) \}^2
$$
称为变量 $x$ 的方差（ variance）。很容易计算得出
$$
\sigma ^2(x) = \mathrm{E}(x^2) - \{ \mathrm{E} (x) \}^2
$$
如果 $f(x)$ 有界，即
$$
|f(x)| \le K
$$
则可以找到 $\mathrm{P} (|x| \ge a)$ 的下界。
$$
\mathrm{E} (f(x)) = \int_E f(x) \mathrm{P}(dE) =  \int_{\{ |x| < a \}} f(x) \mathrm{P}(dE) +  \int_{\{ |x| \ge a \}} f(x) \mathrm{P}(dE) \le f(a) \mathrm{P}(|x| < a) + K \mathrm{P}(|x| \ge a) \le f(a) + K \mathrm{P}(|x| \ge a)
$$


因此
$$
\tag{7}
\mathrm{P} (|x| \ge a) \ge \frac{\mathrm{E}\{f(x\} - f(a) }{K}
$$
如果不是 $f(x)$ 有界，而是 $x$ 本身有界，即
$$
|x| \le M
$$
则 $f(x) \le f(M)$，并且可得如下不等式
$$
\tag{8}
\mathrm{P} (|x| \ge a) \ge \frac{\mathrm{E}\{f(x)\} - f(a) }{f(M)}
$$
当 $f(x) = x^2$ 时，由

公式 $(8)$ 可得
$$
\tag{9}
\mathrm{P} (|x| \ge a) \ge \frac{\mathrm{E}(x^2) - a^2 }{M^2}
$$





### 收敛判据

假定
$$
\tag{1}
x_1, x_2, \dots, x_n, \dots
$$
为随机变量序列，$f(x)$ 为非负偶函数， 且当 $x > 0$ 时 $f(x)$ 单调递增[^4.5]，则以下定理成立：

**定理 I**：序列 $(1)$ 依概率收敛的充分条件是：对任意 $\epsilon > 0$，总存在 $n$，使得对每一个 $p > 0$，以下不顾吃成立：
$$
\tag{2}
\mathrm{E} \{ f(x_{n + p} - x_n) \} < \epsilon 
$$
**定理 II**：序列 $(1)$ 依概率收敛到随机变量 $x$ 的充分条件是：
$$
\tag{3}
\lim_{n \rightarrow + \infin} \mathrm \{ f(x_n - x) \} = 0
$$
**定理 III**：如果 $f(x)$ 有界且连续，并且 $f(0) = 0$，则定理 **I** 和 **II** 中的充分条件也为必要条件。 

**定理 IV**：如果 $f(x)$ 连续，$f(0) = 0$，且序列 $x_1, x_2, \dots, x_n, \dots, x$ 是有界的，则定理 **I** 和 **II** 中的充分条件也为必要条件。 

由定理 **II** 和定理 **IV** 可得定理 **V**：

**定理 V**：序列 $(1)$ 依概率收敛的充分条件是：
$$
\tag{4}
\lim \mathrm{E} (x_n - x)^2 = 0
$$
如果序列 x1,x2,…,xn,…,x 是有界的，则此充分条件也为必要条件。

定理 **I** - **IV** 的证明见 Slutsky [1]、Fréchet [1]。不过，由上一节的公式 $(3)$ 和 $(8)$ 也可立即推得这些定理。



### 数学期望对参数的微分和积分

现在将每个基本事件 $\xi$ 对应到一个定义在实变量 $t$ 上的确定的实函数 $x(t)$。如果对于每一个固定的 $t$，变量 $x(t)$ 是随机变量，则称 $x(t)$ 为随机函数（random variable）。现在的问题是，在什么条件下数学期望符号（$\mathrm{E}(x)$）可以与积分符号（$\int$）及微分符号（$dx$）互换。接下来的两个定理，尽管无法穷尽这个问题，但它们可以在许多简单的情况下给出足够令人满意的答案。

**定理 I**：如果对于任意的 $t$，数学期望 $\mathrm{E}[x(t)]$ 是有限的，且 $x(t)$ 总是可微的，同时 $x(t)$ 对 $t$  的导数 $x'(t)$ 的绝对值总是小于某个常数 $M$，则有
$$
\frac{d}{dt} \mathrm{E} [x(t)] = \mathrm{E}[x'(t)]
$$
**定理 II**：如果 $x(t)$ 的绝对值总是小于某个常数 $K$，且黎曼可积（integrable in the Riemann sense[^*]），并且 $\mathrm{E} [x(t)]$ 也是黎曼可积的，则
$$
\int_a ^b \mathrm{E} (x(t)) dt = \mathrm{E} [ \int_a ^b x(t) dt ]
$$
**定理 I 的证明**：假设 $x'(t)$ 为以下随机变量的极限：
$$
\frac{x(t + h) - x(t)}{h} \qquad h = 1, \frac{1}{2}, \dots, \frac{1}{n}, \dots
$$
 $x'(t)$ 也是随机变量。因为 $x'(t)$ 是有界的，所以数学期望 $\mathrm{E} [x'(t)]$ 存在（第 2 节，数学期望的性质 VII）。现在固定 $t$，记以下事件为 $A$：
$$
| \frac{x(t + h) - x(t)}{h} - x'(t) | > \epsilon
$$
对于每一个 $\epsilon > 0$，当 $h \rightarrow 0$ 时，概率 $\mathrm{P} (A)$ 趋近于 $0$。因为
$$
| \frac{x(t + h) - x(t)}{h} | \le M
$$
和 $|x(t)| \le M$ 总是成立的【前一个有定理 I 中导数有界可知，第二个为何总是成立？】，并且事件 $A$ 的对立事件 $\bar{A}$ 为
$$
| \frac{x(t + h) - x(t)}{h} - x'(t) | \le \epsilon
$$
因此
$$
| \frac{\mathrm{E} [x(t + h)] - \mathrm{E} [x(t)]}{h} - \mathrm{E} [x'(t)] | \le \mathrm{E} | \frac{x(t + h) - x(t)}{h} - x'(t) | = \mathrm{P} (A) \mathrm{E}_A | \frac{x(t + h) - x(t)}{h} - x'(t) | + \mathrm{P} (\bar{A}) \mathrm{E}_{\bar{A}} | \frac{x(t + h) - x(t)}{h} - x'(t) | \le 2 M \mathrm{P} (A) + \epsilon
$$

选择任意的 $\epsilon > 0$，对于任何足够小的 $h$，$\mathrm{P}(A)$ 可以任意小。因此有
$$
\frac{d}{dt} \mathrm{E} [x(t)] = \lim _{h \rightarrow 0} \frac{\mathrm{E} [x(t + h)] - \mathrm{E} [x(t)]}{h} = \mathrm{E} [x'(t)]
$$
定理 I 得证。

**定理 II 的证明**：令
$$
S_n = \frac{1}{h} \sum_{k = 1} ^{k = n} x(t + kh), \qquad h = \frac{b - a}{n}
$$
因为 $S_n$ 收敛于 $J = \int_a ^b x(t) dt$，我们可以选择任意的 $\epsilon > 0$ 和 $N$，使得当 $n \ge N$ 时，以下不等式成立
$$
\mathrm{P} (A) = \mathrm{P} \{ |S_k - J| > \epsilon \} < \epsilon
$$
如果令
$$
S_n^* = \frac{1}{h} \sum_{k = 1} ^{k = n} \mathrm{E} [x(t + kh)] = \mathrm{E} (S_n)
$$
则
$$
|S_n^* - \mathrm{E}(J)| = | \mathrm{E}(S_n - J) | \le \mathrm{E} |S_n - J| = P(A) \mathrm{E}_A |S_n - J| + \mathrm{P} (\bar{A}) \mathrm{E}_{\bar{A}} |S_n - J|_i \le 2K \mathrm{P} (A) + \epsilon \le (2K + 1) \epsilon
$$
因此 $S_n^*$ 收敛于 $\mathrm{E}(J)$，由此得
$$
\int_a ^b \mathrm{E} [x(t)] dt = \lim S_n^* = \mathrm{E}(J)
$$
定理 II 可以很容易推广到二重、三重以及更高阶的多重积分。此处给出这个定理在几何概率中的一个应用。令 $G$ 为某一平面上的可测度区域，该平面的形状是随机的。换种方式表述即为，对概率域中的每个基本事件 $\xi$ ，为其指定一个可测平面 $G$。将区域 $G$ 的面积记为 $J$，点 $(x, y)$ 属于区域 $G$ 的概率记为 $\mathrm{P}(x, y)$。则
$$
\mathrm{E} (J) = \int \int \mathrm{P} (x, y) dx dy
$$
要证明这一关系，只需记
$$
J = \int \int f(x, y) dx dy \\
\mathrm{P}(x, y) = \mathrm{E} f(x, y)
$$
其中 $f(x, y)$ 是区域 $G$ 的示性函数（characteristic function）（在 $G$ 上 $f(x, y) = 1$，在 $G$ 外 $f(x, y) = 0$）[^4.6]。












[^*]: 对于定义在闭区间 $[a, b]$ 上的有界函数 $f(x)$，若以下极限存在且唯一，则称 $f(x)$ 在 $[a, b]$ 上黎曼可积：

$$
\int_a^b f(x) \, dx = \lim_{\|P\| \to 0} \sum_{i=1}^n f(\xi_i) \Delta x_i
$$

 其中：

- 分割（Partition）：将区间 $[a, b]$ 分为子区间 $[x_{i - 1}, x_i]$，记分割为 $P = \{ x_0, x_1, \dots, x_n \}$。
- 样本点（Tag）：在每个子区间中任取一点 $\xi _i \in [x_{i - 1}, x_i]$。
- 黎曼和（Riemann Sum）：$\sum_{i=1}^n f(\xi_i) \Delta x_i$，其中 $\Delta x_i = x_i - x_{i - 1}$。
- 分割的模（Norm）：$||P|| = \max \Delta x_i$，表示最大子区间长度。

当所有可能的黎曼和在 $||P|| \rightarrow 0$ 时趋于同一极限，则此极限为黎曼积分。





[^4.1]: 和第三章第 $5$ 节一样，本章及之后的章节的研究内容都是在波莱尔概率域上开展的。
[^4.2]: FRÉCHET, Sur l’intégrale d’une functionnelle étendue à un ensemble abstrait, Bull. Soc. Math. France v. 43, 1915, p. 248.
[^4.3]: 假设 $y$ 是一个随机变量，按照积分理论的术语来说，$y$ 对于 $\mathcal{E}$ 是可测的。

[^*]: Stieltjes积分，以荷兰数学家**托马斯·约翰内斯·斯蒂尔杰斯（Thomas Joannes Stieltjes）**的名字命名，是黎曼积分的一种推广。它允许对一个函数进行积分，而不仅仅是对变量（如黎曼积分中的 $dx$）进行积分。这使得Stieltjes积分在概率论、泛函分析和物理学等领域中成为一个强大的工具。

[^4.4]: 参考 V. GLIVENKO, Sur les valeurs probables de fonctions, Rend. Accad. Lincei v. 8, 1928, pp. 480-483.

[^4.5]: 因此当 $x \ne 0$ 时，$f(x) > 0$。

[^4.6]: 参考A. KOLMOGOROV and M. LEONTOVICH, Zur Berechnung der mittleren Brownschen Fläche, Physik. Zeitschr. d. Sovietunion, v. 4, 1933.

