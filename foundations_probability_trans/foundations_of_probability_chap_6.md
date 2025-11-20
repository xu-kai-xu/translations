## 独立性；大数定律



### 独立性

**定义 $1$**：$u$ 和 $v$ 是基本事件 $\xi$ 的两个函数。对于 $\mathcal{E}^{(u)}$ 中的集合 $A$, 和 $\mathcal{E}^{(v)}$ 中的集合 $B$，如果以下等式成立，则称 $u$ 和 $v$ 是相互独立的。
$$
\tag{1}
\mathrm{P} ( u \sub A, v \sub B ) = \mathrm{P} ( u \sub A ) \mathrm{P} ( v \sub B ) = \mathrm{P}^{(u)} (A) \mathrm{P}^{(v)} (B)
$$
如果集合 $E^{(u)}$ 和 $E^{(v)}$ 仅由有限个元素组成
$$
E^{(u)} = u_1 + u_2 + \dots + u_n
\\
E^{(v)} = v_1 + v_2 + \dots + v_n
$$
则 $u$ 和 $v$ 独立性的定义与以下划分的定义是相同的（见第五章第 $1$ 节）
$$
E = \sum_k \{ u = u_k \}
\\
E = \sum_k \{ v = u_k \}
$$
$u$ 和 $v$ 独立的充要条件如下：对 $\mathcal{E}^{(u)}$ 中任意选择的集合 $A$，如下等式几乎必定成立
$$
\tag{2}
\mathrm{P}_v (u \sub A) = \mathrm{P} (u \sub A)
$$
当 $\mathrm{P}^{(v)} (B) = 0$ 时，公式 $(1)$ 和公式 $(2)$ 都满足，接下来只需证明在 $\mathrm{P}^{(v)} (B) > 0$ 时它们的等价性即可。此时公式 $(1)$ 等价于以下关系
$$
\tag{3}
\mathrm{P} _{\{ v \sub B \}} (u \sub A) = \mathrm{P} (u \sub A)
$$
并因此等价于以下关系
$$
\tag{4}
\mathrm{E}_{\{ v \sub B \}} \mathrm{P}_v(u \sub A) = \mathrm{P} (u \sub A)
$$
另一方面，显然公式 $(4)$ 可以由公式 $(2)$ 推出。相反地，因为 $\mathrm{P}_v (u \sub A)$ 在概率零的意义下（to within probability zero）由公式 $(4)$ 唯一确定，所以公式 $(2)$ 也可以由公式 $(4)$ 推出。

**定义 $2$**：令 $M$ 为基本事件 $\xi$ 的函数 $u_{\mu} (\xi)$ 的集合。当以下条件得到满足时，称这些函数在整体上是相互独立的（mutually independent in their totality）。令 $M'$ 和 $M''$ 为 $M$ 的两个不相交的子集，并且令 $A'$（或 $A''$）为 $\mathcal{E}$ 中的集合，$A'$ 由 $M'$  中的关系定义（同理，$A''$ 由 $M''$ 中的关系定义），则有以下公式：
$$
\mathrm{P} (A' A'') = \mathrm{P} (A') \mathrm{P} (A'')
$$

所有 $M'$（或 $M''$）构成的 $u_{\mu}$ 的总体可以视为部分函数 $u'$（或 $u''$）的坐标。定义 $2$ 仅要求对于任意选取的不相交集合$M'$ 和 $M''$，函数 $u'$ 和 $u''$在定义 $1$ 的意义下相互独立。

如果 $u_1, u_2, \dots, u_n$ 是相互独立的，并且 $A_k$ 属于对应的 $\mathcal{E}^{uk}$（由归纳法可知）， 则在任何情况下都有如下关系
$$
\tag{5}
\mathrm{P} \{ u_1 \sub A_1, u_2 \sub A_2, \dots, u_n \sub A_n \} = \mathrm{P} (u_1 \sub A_1) \mathrm{P} (u_2 \sub A_2) \dots \mathrm{P} (u_n \sub A_n)
$$
但一般来说，上式不足以保证 $u_1,u_2, \dots, u_n$ 的相互独立性。

公式 $(5)$ 可以很容易地推广到可数无限个乘积的情况。

即使任意有限群 $(u_{\mu_1}, u_{\mu_2}, \dots, u_{\mu_k})$ 中的 $u_{\mu_k}$ 两两相互独立，也不能推出所有的 $u_{\mu}$ 都是相互独立的。

最后，可以很容易地注意到，函数 $u_{\mu}$ 的相互独立性实际上是对应划分 $\mathcal{U}_{u_{\mu}}$ 的性质。进一步地，如果 $u'_{\mu}$ 是对应的 $\mathcal{U}_{\mu}$ 的单值函数，  则由 $u_{\mu}$ 的相互独立性可得 $u'_{\mu}$ 的相互独立性。



### 独立随机变量

如果 $x_1, x_2, \dots, x_n$ 是相互独立的随机变量，则根据本章上一节的公式 $(2)$ 可得以下公式
$$
\tag{1}
F^{(x_1, x_2, \dots, x_n)} (a_1, a_1, \dots, a_n) = F^{(x_1)} (a_1) F^{(x_2)} (a_2) \dots F^{(x_n)} (a_n)
$$
如果此时域 $\mathcal{E}^{(x_1, x_2, \dots, x_n)}$ 仅包含空间 $R^n$ 的波莱尔集，则公式 $(1)$ 也是变量 $x_1, x_2, \dots, x_n$ 相互独立的充分条件。

**证明**

令 $x' = (x_{i_1}, x_{i_2}, \dots, x_{i_n})$，$x'' = (x_{j_1}, x_{j_2}, \dots, x_{j_n})$ 为变量 $x_1, x_2, \dots, x_n$ 的两个不相交的子系统。需要证明，由公式 $(1)$ 可得，对所有的 $R^k$（或 $R^m$）中波莱尔集合 $A'$ 和 $A''$，以下公式成立
$$
\tag{2}
\mathrm{P} (x' \sub A', x'' \sub A'') = \mathrm{P} (x' \sub A') \mathrm{P} (x'' \sub A'')
$$
当 $A'$ 和 $A''$ 是以下形式的集合时，公式 $(2)$ 显然成立
$$
A' = \{ x_{i_1} < a_1, x_{i_2} < a_2, \dots, x_{i_k} < a_k \} \\
A'' = \{ x_{j_1} < b_1, x_{j_2} < b_2, \dots, x_{j_k} < b_m \} 
$$
可以证明集合 $A'$ 和 $A''$ 的这一性质在和与差的运算下保持不变。由此可得，公式 $(2)$ 对所有的波莱尔集都成立。

接下来令 $x = \{ x_{\mu} \}$ 为一任意的（通常为无限的）随机变量集合。如果域 $\mathcal{E}^{(x)}$ 恰巧与域 $B \mathcal{E}^M$（$M$ 为所有 $\mu$ 的集合），以下公式的全体是变量 $x_{\mu}$ 相互独立的充要条件
$$
\tag{3}
F_{(\mu_1, \mu_2, \dots, \mu_n)} (a_1, a_1, \dots, a_n) = F_{\mu_1} (a_1) F_{\mu_2} (a_2) \dots F_{\mu_n} (a_n)
$$
此条件的必要性可由公式 $(1)$ 推得，接下来证明此条件也为充分条件。令 $M'$ 和 $M''$ 为集合 $M$ 的两个互不相交的子集，令 $A'$（或 $A''$）为由 $M'$（或 $M''$）中的 $\mu$ 所对应的随机变量 $x_{\mu}$ 中的关系定义的 $B \mathcal{E}^{M}$ 中的集合，则有
$$
\tag{4}
\mathrm{P} (A' A'') = \mathrm{P}(A') \mathrm{P}(A'')
$$
如果 $A'$ 和 $A''$ 是圆柱集，则我们此时处理的是变量 $x_{\mu}$ 的有限集合。公式 $(4)$ 代表之前结论（公式 $(2)$）的一个简单结果。因为公式 $(4)$ 对于集合 $A'$ 和 $A''$ 的和和差也是成立的，所以证明公式 $(4)$ 对 $B\mathcal{E}^M$ 中的所有集合也成立。

现在对集合 $M$ 中的每一个 $\mu$，给定一个先验分布函数 $F_{\mu} (a)$。此时可以构造一个概率域，其中的随机变量 $x_{\mu}$（$\mu$ 表示 $M$ 中所有的值） 是相互独立的。此概率域中的每一个 $x_{\mu}$ 都有对应的先验分布函数 $F_{\mu}(a)$。为证明这一点，仅需在基本集合 $E$ 中取 $R^M$、在波莱尔集 $\mathcal{E}$ 中取 $B \mathcal{E}^M$，并按照公式 $(3)$ 定义分布函数 $F_{\mu_1 \mu_2 \dots \mu_n}$（见第三章第 $4$ 节）。

需要指出，根据每个 $x_{\mu}$ 的有限群的相互独立性（公式 $(3)$），可得波莱尔集 $B \mathcal{E}^M$ 上所有集合的相互独立性。在概率论的某些扩展框架下，此类性质可能失效。

最后在本章结尾，给出两个随机变量独立性的几个判断准则。

如果随机变量 $x$ 和 $y$ 相互独立，且 $\mathrm{E}(x)$ 和 $\mathrm{E}(y)$ 是有限的，则几乎必然有以下公式
$$
\tag{5}
\mathrm{E}_x (y) = \mathrm{E} (y) \\
\mathrm{E}_y (x) = \mathrm{E} (x)
$$
以上公式为条件数学期望的第二种定义的直接结果（第五章第 $4$ 节中的公式 $(10)$ 和公式 $(11)$）。因此，在独立性的前提下
$$
f^2 = \frac{\mathrm{E} [y - \mathrm{E}_x (y)] ^2}{\sigma ^2 (y)} = \frac{\sigma ^2 [\mathrm{E} _x (y)]}{\sigma ^2 (y)}
\\
g^2 = \frac{\mathrm{E} [x - \mathrm{E}_y (x)] ^2}{\sigma ^2 (x)} = \frac{\sigma ^2 [\mathrm{E} _y (x)]}{\sigma ^2 (x)}
$$
上面两个公式都等于 $0$（假设 $\sigma^2(x) > 0$ 且 $\sigma^2(y) > 0$）。$f^2$ 称为 $y$ 相对于 $x$ 的相关比（correlation ratio），$g^2$ 称为 $x$ 相对于 $y$ 的相关系数（见 Pearson 的成果）。

由公式 $(5)$ 可进一步得到
$$
\tag{6}
\mathrm{E} (xy) = \mathrm{E} (x) \mathrm{E} (y)
$$
为证明上式，应用第五章第 $4$ 节的公式 $(15)$：
$$
\mathrm{E} (xy) = \mathrm{E} \mathrm{E}_x (xy) = \mathrm{E} [x \mathrm{E}_x (y)] = \mathrm{E} [x \mathrm{E}(y)] = \mathrm{E}(y) \mathrm{E} (x)
$$
因此当 $x$ 和 $y$ 相互独立时
$$
r = \frac{\mathrm{E}(x, y) - \mathrm{E}(x) \mathrm{E}(y)}{\sigma(x) \sigma(y)}
$$
也等于 $0$；其中 $r$ 称为 $x$ 和 $y$ 的相关系数（correlation coefficient）。

如果两个随机变量 $x$ 和 $y$ 满足公式 $(6)$，则称它们为不相关的（uncorrelated）。对于以下和式
$$
S = x_1 + x_2 + \dots + x_n
$$
其中 $x_1, x_2, \dots, x_n$ 两两互不相关，可以很容易计算
$$
\tag{7}
\sigma ^2(S) = \sigma ^2(x_1) + \sigma ^2(x_2) + \dots + \sigma ^2(x_n)
$$
特别地，公式 $(7)$ 对于独立变量 $x_k$ 是成立的。



### 大数定律

对于随机变量 $s$ 的序列
$$
s_1, s_2, \dots, s_n, \dots
$$
如果存在数值序列
$$
d_1, d_2, \dots, d_n, \dots
$$
使得对任意的正的 $\epsilon$，当 $n \rightarrow \infin$ 时，概率
$$
\mathrm{P} \{ |s_n - d_n| \ge \epsilon \}
$$
收敛到 $0$，则称随机变量 $s$ 的序列是稳定的。如果所有的 $\mathrm{E} (s_n)$ 都存在并且令
$$
d_n = \mathrm{E}(s_n)
$$
则此稳定性是正规的（the stability is normal）。

如果所有的 $s_n$ 都是一致有界的（uniformly bounded），则根据下式
$$
\tag{1}
\mathrm{P} \{ |s_n - d_n| \ge \epsilon \} \rightarrow 0 \qquad n \rightarrow + \infin
$$
可得
$$
|\mathrm{E}(s_n) - d_n| \rightarrow 0  \qquad n \rightarrow + \infin 
$$
并且可得
$$
\tag{2}
\mathrm{P} \{ |s_n - \mathrm{E}(s_n)| \ge \epsilon \} \rightarrow 0 \qquad n \rightarrow + \infin
$$
因此有界稳定序列的稳定性必然是正规的。

令
$$
\mathrm{E} (s_n - \mathrm{E}(s_n)) ^2 = \sigma ^2 (s_n) = \sigma_n ^2
$$
则由切比雪夫不等式（Tchebycheff inequality）可得
$$
\mathrm{P} \{ |s_n - d_n| \ge \epsilon \} \le \frac{\sigma ^2 _n}{\epsilon ^2}
$$
因此，马尔可夫条件（the Markov Condition）
$$
\tag{3}
\sigma^2 _n \rightarrow 0 \qquad  \qquad n \rightarrow + \infin
$$
是正规稳定的充分条件。

如果 $s_n - \mathrm{E}(s_n)$ 是一致有界的，即
$$
|s_n - \mathrm{E}(s_n)| \le M
$$
则由第四章第 $3$ 节的公式 $(9)$ 可得
$$
\mathrm{P} \{ | s_n - \mathrm{E}(s_n) | \ge \epsilon \} \ge \frac{\sigma^2 _n - \epsilon ^2}{M^2}
$$
因此这种情况下马尔可夫条件（公式 $(3)$）仍然是序列 $s_n$ 稳定的必要条件。

如果
$$
s_n = \frac{x_1 + x_2 + \dots + x_n }{n}
$$
并且变量 $x_n$ 两两互不相关（uncorrelated in pairs），则有
$$
\sigma^2 _n = \frac{1}{n^2} \{ \sigma^2(x_1) + \sigma^2(x_2) + \dots + \sigma^2(x_n) \}
$$
所以此时以下条件是随机变量序列 $s_n$ 的算数平均正规稳定的充分条件（切比雪夫定理[^6.&]）
$$
\tag{4}
n^2 \sigma_n ^2 = \sigma^2(x_1) + \sigma^2(x_2) + \dots + \sigma^2(x_n)  = o(n^2)
$$
特别地，如果所有的 $x_n$ 都是一致有界的，则公式 $(4)$ 中的条件得到满足。

此定理可以推广到弱相关（weakly correlated）变量 $x_n$ 的情形。假设变量 $x_m$ 和 $x_n$ 的相关系数 $r_{mn}$[^6.1] 满足以下不等式
$$
r_{mn} \le c (|n - m|)
$$
并且
$$
C_n = \sum ^{k = n - 1} _{k = 0} c(k)
$$
则 $s$ 的算数平均的正规稳定性的充分条件是[^6.2]
$$
\tag{5}
C_n \sigma^2 _n = o(n^2)
$$

在 $x_n$ 为独立和项[^6.*]（independent summands）的情况下，可以给出 $s_n$ 的算数平均稳定性的充要条件。 对每一个 $x_n$，都存在一个常数 $m_n$（$x_n$ 的中位数），满足如下条件
$$
\mathrm{P} (x_n < m_n) \le \frac{1}{2} \\
\mathrm{P} (x_n > m_n) \le \frac{1}{2}
$$
令
$$
x_{nk} = x_k \qquad \text{if} \quad  |x_k - x_m| \le n ,\\
x_{nk} = 0 \qquad \text{otherwise}, \\
s_n^* = \frac{x_{n1} + x_{n2} + \dots + x_{nn} }{n}
$$
则以下公式分别为 $s_n$ 稳定的必要和充分条件[^6.3]
$$
\tag{6}
\sum ^{k = n} _{k = 1} \mathrm{P} \{ |x_k - m_k| > n \} = \sum ^{k = n} _{k = 1} \mathrm{P} (x_{nk} \ne x_k) \rightarrow 0, \qquad n \rightarrow + \infin
$$

$$
\tag{7}
\sigma^2 (s^*_n) = \sum ^{k = n} _{k = 1}  \sigma^2 (x_{nk}) = o(n^2)
$$

在此假设常数 $d_n$ 等于 $\mathrm{E}(s_n ^*)$，则在（并且只在）以下条件成立时，$s_n$ 的稳定是正规的。
$$
\mathrm{E}(s^*_n) - \mathrm{E}(s_n) \rightarrow 0, \qquad n \rightarrow + \infin
$$
如果假设 $s_n$ 以某种方式依赖于任意 $n$ 次试验的结果（如下），则可以得到切比雪夫定理更进一步的推广结果。
$$
\mathcal{U}_1, \mathcal{U}_2, \dots, \mathcal{U}_n
$$
这样当所有这 $n$ 次试验的每个结果都确定后，$s_n$ 也随之确定。所有这些被称为**大数定律**（the law of large numbers）的定理，其大体思路在于，若对于较大的 $n$，变量 $S_n$ 对每个单独的试验 $\mathcal{U}_k \quad (k = 1, 2, \dots, n)$ 的依赖性非常弱，则变量 $S_n$ 是稳定的。如果把
$$
\beta ^2 _{nk} = \mathrm{E} [ \mathrm{E}_{\mathcal{U}_1, \mathcal{U}_2, \dots, \mathcal{U}_k} (s_n) - \mathrm{E} _{\mathcal{U}_1, \mathcal{U}_2, \dots, \mathcal{U}_{k - 1}} (s_n)]^2
$$
作为衡量 $s_n$ 对试验 $\mathcal{U_k}$ 的依赖性的一个合理的测度，则上述提到的大数定律的大体思路可在以下论证后更加坚实具体[^6.4]。

令
$$
z_{nk} = \mathrm{E}_{\mathcal{U}_1, \mathcal{U}_2, \dots, \mathcal{U}_k} (s_n) - \mathrm{E} _{\mathcal{U}_1, \mathcal{U}_2, \dots, \mathcal{U}_{k - 1}} (s_n)
$$
则
$$
s_n - \mathrm{E}(s_n) = z_1 + z_2 + \dots + z_n \\
\mathrm{E}(z_{nk}) = \mathrm{E} [\mathrm{E}_{\mathcal{U}_1, \mathcal{U}_2, \dots, \mathcal{U}_k} (s_n) - \mathrm{E} _{\mathcal{U}_1, \mathcal{U}_2, \dots, \mathcal{U}_{k - 1}} (s_n)] = \mathrm{E}(s_n) - \mathrm{E}(s_n) = 0 \\
\sigma^2 (z_{nk}) = \mathrm{E} (z^2 _{nk}) = \beta ^2 _{nk}
$$


并且可以很容易计算出随机变量 $z_{nk} \quad (k = 1, 2, \dots, n)$ 是不相关的。令 $i < k$，则[^6.5]
$$
\mathrm{E}_{\mathcal{U}_1, \mathcal{U}_2, \dots, \mathcal{U}_{k - 1}} (z_{ni} z_{nk}) = z_{ni} \mathrm{E}_{\mathcal{U}_1, \mathcal{U}_2, \dots, \mathcal{U}_{k - 1}} (z_{nk}) = z_{ni}  \mathrm{E}_{\mathcal{U}_1, \mathcal{U}_2, \dots, \mathcal{U}_{k - 1}} [ \mathrm{E}_{\mathcal{U}_1, \mathcal{U}_2, \dots, \mathcal{U}_k} (s_n) - \mathrm{E} _{\mathcal{U}_1, \mathcal{U}_2, \dots, \mathcal{U}_{k - 1}} (s_n) ] = z_{ni} [ \mathrm{E}_{\mathcal{U}_1, \mathcal{U}_2, \dots, \mathcal{U}_{k - 1}} (s_n) - \mathrm{E} _{\mathcal{U}_1, \mathcal{U}_2, \dots, \mathcal{U}_{k - 1}} (s_n) ] = 0
$$
因此
$$
\mathrm{E}(z_{ni} z_{nk}) = 0
$$
由此可得
$$
\sigma^2 (s_n) = \sigma^2 (z_{n1}) + \sigma^2 (z_{n2}) + \dots + \sigma^2 (z_{nn}) = \beta^2 _{n1} + \beta^2 _{n2} + \dots + \beta^2 _{nn}
$$
因此，以下公式
$$
\beta^2 _{n1} + \beta^2 _{n2} + \dots + \beta^2 _{nn} \rightarrow 0 \qquad n \rightarrow 0
$$
为 $s_n$ 正规稳定的充分条件。



### 关于数学期望概念的说明

由前文内容可知，随机变量 $x$ 的数学期望定义为
$$
\mathrm{E} (x) = \int _{E} \mathrm{P}(dE) = \int ^{+ \infin} _{- \infin} a d F^{x}(a)
$$
其中上式右侧的积分可解释如下
$$
\tag{1}
\mathrm{E} (x) = \int ^{+ \infin} _{- \infin} a d F^{x}(a) = \lim _{b \rightarrow - \infin, c \rightarrow +\infin} \int _b ^c a d F^{x}(a)
$$
因此，下式可称为一种广义数学期望（a generalized mathematical expectation）
$$
\tag{2}
\mathrm{E}^* (x) = \lim _{b \rightarrow + \infin} \int _{-b} ^{+b} a \, d F^{x}(a)
$$
当然在这种情况下会失去数学期望的一些简单性质。丽日此时
$$
\mathrm{E} (x + y) = \mathrm{E}(x) + \mathrm{E}(y)
$$
并不总是成立。以这种方式的推广几乎是难以接受的。但如果加上一些限制性的补充条件的话，定义 $(2)$ 就变得完全自然且实用了。

可以按如下方式讨论此问题，令
$$
x_1, x_2, \dots, x_n, \dots
$$
为相互独立的随机变量序列，并且这个随机变量序列与随机变量 $x$ 有相同的分布函数，即 $F^{(x)}(a) = F^{(x_n)}(a), \quad (n = 1, 2, \dots)$。进一步令
$$
s_n = \frac{x_1 + x_2 + \dots + x_n}{n}
$$
此时请问，是否存在一个常量 $\mathrm{E}^* (x)$，满足对任意的 $\epsilon > 0$，下式都成立
$$
\tag{3}
\lim \mathrm{P} (| s_n - \mathrm{E}^*(x) | > \epsilon) = 0, \qquad n \rightarrow + \infin 
$$
答案：如果常量 $\mathrm{E}^*(x)$ 存在，则它可以由公式 $(2)$ 表示。公式 $(3)$ 成立的充要条件为：1）公式 $(2)$ 表示的极限存在；2）公式 $(4)$ 表示的关系成立。
$$
\tag{4}
\mathrm{P} (|x| > n) = o(\frac{1}{n})
$$
为证明此结论，我们应用如下定理：

> 条件 $(4)$ 是算数平均 $s_n$ 稳定的充要条件。

当 $s_n$ 稳定时令[^6.6]
$$
d_n = \int ^{+n} _{-n} a F^{(x)}(a)
$$
如果存在公式 $(1)$ 定义的数学期望，则条件 $(4)$ 总是可以得到满足[^6.7]。因为此时 $\mathrm{E}(x) = \mathrm{E}^* (x)$，所以条件 $(3)$ 实际上确实定义了数学期望概念的一种推广。对于此广义的数学期望，性质 I - VII（第四章第 $2$ 节）仍然成立。但 $\mathrm{E}^*(x)$ 的存在并不能推出 $\mathrm{E}^* |x|$ 的存在。

为证明新的数学期望的概念比先前的概念更具普遍性，只需给出以下示例即可。令概率密度函数 $f^{(x)}(a)$ 如下
$$
f^{(x)} (a) = \frac{C}{(|a| + 2)^2 \ln (|a| + 2)}
$$
其中常量 $C$ 由下式确定
$$
\int ^{+ \infin} _{- \infin} f^{(x)} (a) \, da = 1
$$
很容易计算得出，此时条件 $(4)$ 得到满足。由公式 $(2)$ 可得
$$
\mathrm{E}^* (x) = 0
$$
但积分
$$
\int ^{+ \infin} _{- \infin} |a| \, dF^{(x)} (a) \, da = \int ^{+ \infin} _{- \infin} |a| \, f^{(x)} (a) \, da
$$
是发散的。



### 强大数定律；级数收敛

以下序列
$$
s_1, s_2, \dots, s_n, \dots
$$
的随机变量记为 $s_n$ 。如果存在实数序列
$$
d_1, d_2, \dots, d_n, \dots
$$
使得当 $n \to + \infin$ 时随机变量
$$
s_n - d_n
$$
几乎处处趋近于 $0$，则 $s_n$ 是强稳定的。显然由强稳定性可推得普通稳定性（ordinary）。如果令
$$
d_n = \mathrm{E} (s_n)
$$
则此时的强稳定是正规强稳定（normal）。

在切比雪夫情形（见本章第 $3$ 节）下
$$
s_n = \frac{x_1 + x_2 + \dots + x_n}{n}
$$
其中 $x_n$ 是相互独立的。此时以下序列的收敛是 $s_n$ 正规稳定的一个充分条件[^6.8]
$$
\tag{1}
\sum^{\infin}_{n = 1} \frac{\sigma^2(x_n)}{n^2}
$$
从某种意义上看，这个条件是最优的。因为对任意满足以下条件的 $b_n$
$$
\sum^{\infin}_{n = 1} \frac{b_n}{n^2} = + \infin
$$
我们都可以构造一个相互独立的随机变量 $x_n$ 的序列，满足 $\sigma^2(x_n) = b_n$，使得 $s_n$ 不是强稳定的。

如果所有的 $x_n$ 都有相同的分布函数 $F^{(x)} (a)$，则数学期望
$$
\mathrm{E}(x) = \int^{+ \infin} _{- \infin} a \, dF^{(x)} (a)
$$
的存在性是 $s_n$ 强稳定的充分必要条件，并且此时的稳定性总是正规的[^6.9]。

令
$$
x_1, x_2, \dots, x_n, \dots
$$
为相互独立的随机变量，则级数
$$
\tag{2}
\sum^{\infin}_{n = 1} x_n
$$
收敛的概率要么等于 $1$，要么等于 $0$。特别地，当以下两个级数都收敛时，级数 $(2)$ 收敛的概率等于 $1$
$$
\sum^{\infin}_{n = 1} \mathrm{E}(x_n)
\\
\sum^{\infin}_{n = 1} \sigma^2(x_n)
$$
进一步假设
$$
y_n = x_n \qquad \text{in case} \quad |x_n| \le 1
\\
y_n = 0 \qquad \text{in case} \quad |x_n| > 1
$$
则为级数 $(1)$ 依概率 $1$ 收敛的充分必要条件[^6.10]是，以下级数同时收敛
$$
\sum^{\infin}_{n = 1} \mathrm{P} \{ |x_n| > 1 \} \\
\sum^{\infin}_{n = 1} \mathrm{E}(y_n) \\
\sum^{\infin}_{n = 1} \sigma^2 (y_n)
$$




[^6.1]: 显然 $r_{nn}$ 总是等于 $1$。
[^6.&]: 译者注。大 $O$ 记号，表示增长率不超过 $n^2$（可能等于 $n^2$）；小 $o$ 记号，要求更严格，要求增长率必须低于 $n^2$。
[^6.2]:Cf. A. KHINTCHINE, Sur la loi forte des grandes nombres. C. R. de l’acad. sci. Paris v. 186, 1928, p. 285.

[^6.*]:指随机变量序列 $x_n$ 中各项相互独立，且参与求和。
[^6.3]: Cf. A. KOLMOGOROV. Über die Summen durch den Zufall bestimmter unabhängiger Grössen, Math. Ann. v. 99, 1928, pp. 309-319 (corrections and notes to this study, v. 102, 1929 pp. 484-488, Theorem VIII and a supplement on p. 318).
[^6.4]:  Cf. A. KOLMOGOROV. Sur la loi des grandes nombres. Rend. Accad. Lincei v. 9, 1929 pp. 470-474.
[^6.5]: 第五章第 $4$ 节公式 $(15)$ 的应用。

[^6.6]: Cf. A. KOLMOGOROV, Bemerkungen zu meiner Arbeit, “Über die Summen zufälliger Grössen.” Math. Ann. v. 102, 1929, pp. 484-488, Theorem XII.
[^6.7]: Ibid, Theorem XIII.（同上，定理 XIII。）

[^6.8]: Cf. A. KOLMOGOROV, Sur la loi forte des grandes nombres , C. R. Acad. Sci. Paris v. 191, 1930, pp. 910-911.
[^6.9]: The proof of this statement has not yet been published.
[^6.10]: Cf. A. KHINTCHINE and A. KOLMOGOROV, On the Convergence of Series, Rec. Math. Soc. Moscow, v. 32, 1925, p. 668-677.



