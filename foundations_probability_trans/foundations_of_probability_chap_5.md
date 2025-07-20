

## 条件概率和数学期望

### 条件概率

在第一章第 $6$ 节，我们定义了事件 $B$ 相对于试验 $\mathscr{U}$ 的条件概率 $\mathrm{P}_\mathscr{U} (B)$。当时假设 $\mathscr{U}$ 仅包含有限个不同的可能结果。实际上，也可在 $\mathscr{U}$ 包括无限个可能结果的情况下定义 $\mathrm{P}_\mathscr{U} (B)$，例如集合 $E$ 被划分为无限多个不相交的子集的情况。特别地，如果考虑基本事件 $\xi$ 的任意函数 $u$，定义 $u$ 等于常数的集合为划分 $\mathscr{U}_u$  的元素，则可以得到这样一种划分。条件概率 $\mathrm{P}_{\mathscr{U}_u} (B)$ 也记为 $\mathrm{P}_u (B)$。如果对于每一个基本事件 $\xi$ 都定义一个 $u(\xi)$，使得 $u(\xi)$ 表示基本集合 $E$ 的那些划分 $\mathscr{U}$ 中，包括基本事件 $\xi$ 的所有划分的集合，则对基本集合 $E$ 的任意划分 $\mathscr{U}$ 都可以定义为由基本事件 $\xi$ 的函数 $u$ 诱导出的划分 $\mathscr{U}_u$。

当且仅当定义在域 $\mathcal{E}^{(u)}$ 上的 $u$ 和定义在 $\mathcal{E}^{(u’)}$ 上的 $u'$ 之间存在一对一的对应关系 $u' = f(u)$，使得 $u'(\xi)$ 与 $f(u(\xi))$ 相同时，基本事件 $\xi$ 的两个函数 $u$ 和  $u'$ 确定基本集合 $E$ 的两个相同划分 $\mathscr{U}_u = \mathscr{U}_{u'}$。读者可以很容易证明，以下定义的随机变量 $\mathrm{P}_u(B)$ 与 $\mathrm{P}_{u'}(B)$ 在这种情况下是相同的。这实际上是由这两个划分相等决定的，即 $\mathscr{U}_u = \mathscr{U}_{u'}$。

为定义 $\mathrm{P}_u (B)$，需要如下等式：
$$
\tag{1}
\mathrm{P}_{\{ u \sub A \}} (B) = \mathrm{E}_{\{u \sub A\}} [ \mathrm{P}_u (B) ]
$$
如果对所有可能的 $u$，集合 $E^{(u)}$ 都是有限的，则可以很容易证明，对于任意的 $A$ （当 $\mathrm{P}_u (B)$ 的定义如第一章第 $6$ 节所述时），公式 $(1)$ 总是成立的。在一般情况下（当 $\mathrm{P}_u (B)$ 尚未定义时）则需要证明，总存在一个且仅有一个随机变量 $\mathrm{P}_u (B)$ （排除等价随机变量的情况），它是 $u$ 的函数，且对 $\mathcal{E}^{(u)}$ 中任意的 $A$，当满足 $\mathrm{P}^{(u)} > 0$ 时，公式 $(1)$ 也总是成立的。由此在等价意义下确定的 $u$ 的函数 $\mathrm{P}_u (B)$ （determined to within equivalence），称为 $B$ 对于给定 $u$ 的条件概率。当 $u = a$ 时 $\mathrm{P}_u (B)$ 的值记为 $\mathrm{P}_u (a; B)$。

关于 $\mathrm{P}_u (B)$ 的存在性和唯一性的证明：

在公式 $(1)$ 的两边乘上 $\mathrm{P} \{ u \sub A \} = \mathrm{P} ^{(u)} (A)$ 可得：

等式左边：
$$
\mathrm{P} \{ u \sub A \} \mathrm{P}_{\{ u \sub A \}} (B) = \mathrm{P} (B \{ u \sub A \}) = \mathrm{P} (B u^{-1}(A))
$$
等式右边：
$$
\mathrm{P} \{ u \sub A \} \mathrm{E}_{\{u \sub A\}} [ \mathrm{P}_u (B) ] = \int _{\{ u \sub A \}} \mathrm{P}_u (B) \mathrm{P}(dE) = \int_A \mathrm{P}_u (B) \mathrm{P}^{(u)} (dE^{(u)})
$$
由此得出以下等式
$$
\tag{2}
\mathrm{P} (B u^{-1}(A)) = \int_A \mathrm{P}_u (B) \mathrm{P}^{(u)} (dE^{(u)})
$$
反之，由 $(2)$ 也可以推得 $(1)$。当 $\mathrm{P}^{(u)}(A) = 0$ 时，公式 $(1)$ 无意义，公式 $(2)$ 显然成立且无需证明。公式 $(2)$ 因此等价于公式 $(1)$。根据第四章第 $1$ 节的性质 IX 可得，随机变量 $x$ 由所有$\mathcal{E}$ 上的集合的积分的值唯一确定（排除等价随机变量的情况）
$$
\int_A x \mathrm{P} d(E)
$$
因为 $\mathrm{P}_u (B)$ 是定义在概率域 $(\mathcal{E}^{(u)}, \mathrm{P}^{(u)})$ 上的随机变量，可知在不考虑等价随机变量的情况下， $\mathrm{P}_u (B)$ 由公式 $(2)$ 唯一确定。

现在还需要证明 $\mathrm{P}_u (B)$ 是存在的。此处需要用到 Nikodym 定理[^5.1]：

 令 $\mathcal{E}$ 为一个波莱尔域，$\mathrm{P}(A)$ 为定义在 $\mathcal{E}$ 上的非负完全可加集函数（概率理论上的术语为，在 $(\mathcal{E}, \mathrm{P})$ 上的随机变量）；令 $Q(A)$ 为定义在 $\mathcal{E}$ 上的另一个完全可加集函数。由 $Q(A) \ne 0$ 可得 $\mathrm{P}(A) > 0$。于是可知，存在一个在 $\mathcal{E}$ 上可测的函数 $f(\xi)$ （概率论术语，随机变量），且对于每个 $\mathcal{E}$ 中的集合 $A$，满足以下公式
$$
Q(A) \int_A f(\xi) \mathrm{P} (dE)
$$
为将这一定理用于本文的情形，需要证明

1. $Q(A) = \mathrm{P} (B u^{-1}(A))$ 是 $\mathcal{E}^{(u)}$ 上的完全可加集。
2. 由 $Q(A) \ne 0$，可得不等式 $\mathrm{P}^{(u)} (A) > 0$。

首先，由
$$
0 \le \mathrm{P} (B u^{-1}(A)) \le \mathrm{P} (u^{-1}(A)) = \mathrm{P}^{(u)} (A)
$$
可证明第 $2$ 点【大于等于的情况，排除了等于，就只剩下了大于】。

为证明第 $1$ 点，令
$$
A = \sum_n A_n
$$
则
$$
u^{-1}(A) = \sum_n u^{-1}(A_n)
$$
并且
$$
B u^{-1}(A) = \sum_n B u^{-1}(A_n)
$$
因为 $\mathrm{P}$ 完全可加，所以有[^$]
$$
\mathrm{P} (B u^{-1}(A)) = \sum_n \mathrm{P} (B u^{-1} (A_n))
$$
证毕。

由公式 $(1)$ 可得一个重要关系（如果令 $A = E^{(u)}$）

$$
\tag{3}
\mathrm{P} (B) = \mathrm{E} [\mathrm{P}_u(B)]
$$
接下来证明条件概率的两个基本性质。

**定理 I**：以下关系几乎必然成立（It is almost sure）
$$
\tag{4}
0 \le \mathrm{P}_u (B) \le 1
$$
**定理 II**：如果将集合 $B$ 分解为至多可数个集合 $B_n$，则以下等式几乎必然成立
$$
\tag{5}
\mathrm{P}_u (B) = \sum_n \mathrm{P}_u (B_n)
$$
条件概率 $\mathrm{P}_u(B)$ 的这两个性质对应概率函数 $\mathrm{P}(B)$ 的两个性质：$0 \le \mathrm{P}(B) \le 1$ 总是成立，以及 $\mathrm{P}(B)$ 完全可加。这使得我们得以将绝对概率 $\mathrm{P}(B)$ 的许多其他性质推广到条件概率 $\mathrm{P}_u (B)$ 上。但必须时刻谨记，对于确定的集合 $B$，$\mathrm{P}_u (B)$ 是一个仅在等价意义下唯一确定的随机变量（a random variable determined uniquely only to within equivalence）。



定理 I 的证明：与待证命题相反，如果假设在集合 $M \sub E^{(u)}$ 上，且满足 $\mathrm{P}^{(u)} (M) > 0$ 时，不等式 $\mathrm{P}_u (B) \ge 1 + \epsilon, \quad \epsilon > 0$ 总成立，则对应的公式 $(1)$ 变为
$$
\mathrm{P}_{\{ u \sub A \}} (B) = \mathrm{E}_{\{u \sub A\}} [ \mathrm{P}_u (B) ] \ge 1 + \epsilon
$$
显然这是不可能的。同理可证明 $\mathrm{P}_u(B) \ge 0$ 几乎必然成立。

定理 II 的证明：由以下序列的收敛
$$
\sum_n \mathrm{E}| \mathrm{P}_u (B_n) | = \sum_n \mathrm{E}(\mathrm{P}_u (B_n)) = \sum_n \mathrm{P} (B_n) = \mathrm{P}(B)
$$
并结合数学期望的性质 V （第四章第 $2$ 节）可得，序列
$$
\sum_n \mathrm{P}_u (B_n)
$$
几乎必然收敛。因为序列
$$
\sum_n \mathrm{E}_{\{ u \sub A \}}| \mathrm{P}_u (B_n) | = \sum_n \mathrm{E}_{\{ u \sub A \}}(\mathrm{P}_u (B_n)) = \sum_n \mathrm{P}_{\{ u \sub A \}} (B_n) = \mathrm{P}_{\{ u \sub A \}}(B)
$$
对于每一个满足 $\mathrm{P}^{(u)} (A) > 0$ 的集合 $A$ 都是收敛的，所以由刚刚提到的数学期望的性质可得，对于每一个以上提到的集合 $A$，有以下关系：
$$
\mathrm{E}_{\{ u \sub A \}}(\sum_n  \mathrm{P}_u (B_n)) = \sum_n \mathrm{E}_{\{ u \sub A \}}(\mathrm{P}_u (B_n)) = \mathrm{P}_{\{ u \sub A \}}(B) = \mathrm{E}_{\{ u \sub A \}} (\mathrm{P}_u (B_n))
$$
由此，等式 $(5)$ 得证。

在结束本节前，还需要特别指出两种具体情形。首先，如果 $u(\xi) = c$，$c$ 为常数，则 $\mathrm{P}_c (A) = \mathrm{P}(A)$。其次，如果令 $u(\xi) = \xi$， 则可立即推得 $\mathrm{P}_{\xi}(A)$ 在集合 $A$ 上几乎必然为 $1$，在集合 $\bar{A}$ 上几乎必然为 $0$。由此得 $\mathrm{P}_{\xi}(A)$ 为集合 $A$ 的示性函数。





### 波莱尔悖论的解释

取球面上的所有点的集合作为基本集合 $E$，则 $\mathcal{E}$ 为球面上所有波莱尔集合的构成的集合。最终，$\mathrm{P}(A)$ 与集合 $A$ 的测度成正比。现选择两个径向对称的点（two diametrically opposite points）作为球面上的两极，则每一个子午圈（meridian circle）都可以由经度 $\Psi, \quad 0 \le \Psi < \pi$ 唯一定义。因为 $\Psi$ 的取值范围是 $0$ 到 $\pi$（即此处考虑的是完整的子午圈而不仅是半子午圈），纬度 $\Theta$ 必须从 $- \pi$ 到 $+ \pi$ （不是 $-\pi / 2$ 到 $+ \pi / 2$）。波莱尔提出了这样一个问题：给定经度 $\Psi$，给出纬度 $\Theta, \quad - \pi \le \Theta < \pi$ 的条件概率分布。

很容易计算得【如何得到的】
$$
\mathrm{P}_{\Psi} \{ \Theta_1 \le \Theta < \Theta_2 \} = \int ^{\Theta_2} _{\Theta_1} |\cos \Theta| d \Theta
$$
给定 $\Psi$ 时，$\Theta$ 的概率分布不是均匀的。

如果假设”假定 $\xi$ 位于给定子午圈上“时 $\Theta$ 的条件概率必须是均匀的，则此处产生了矛盾。

这表明，针对一个**概率为零的孤立假设**（例如单一点或零测集）来定义条件概率的概念是不可行的。因为只有当我们将子午圈视为整个球面按给定极点分解为若干子午圈这一分解结构中的一个元素时，才能获得该子午圈上 $\Phi$ 的概率分布。

### 随机变量的条件概率

如果 $X$ 是随机变量，$\mathrm{P}_x(B)$ 为 $X$ 的函数，且 $\mathrm{P}_x (B)$ 是波莱尔可测的，则 $\mathrm{P}_x(B)$ 可以以一种基本的方式定义。我们可以以另一种形式重写第 $1$ 节的公式 $(2)$：
$$
\tag{1}
\mathrm{P}(B) \mathrm{P}_B ^{(x)}(A) = \int_A \mathrm{P}_x (B) \mathrm{P}^{(x)} (dE)
$$
由此可由公式 $(1)$ 立刻得出
$$
\tag{2}
\mathrm{P}(B) F_B ^{(x)}(a) = \int_{-\infin} ^{a} \mathrm{P}_x (a;B) dF^{(x)} (a)
$$
根据勒贝格（Lebesgue）的一个定理[^5.2]，由公式 $(2)$ 可得
$$
\tag{3}
\mathrm{P}_x (a;B) = \mathrm{P}(B) \lim \frac{F^{(x)}_B (a+h) - F^{(x)}_B (a)}{F^{(x)} (a+h) - F^{(x)} (a)}, \qquad h \rightarrow 0
$$
除在满足 $\mathrm{P}^{(x)} (H) = 0$ 的点集 $H$ 外，公式 $(3)$ 总是成立。

$\mathrm{P}_x (a;B)$ 在本章第 $1$ 节定义（除在满足 $\mathrm{P}^{(x)} (G)$ 的集合 $G$ 之外）。如果现在把公式 $(3)$ 作为 $\mathrm{P}_x (a;B)$ 的定义（当公式 $(3)$ 右边的极限不存在时，令 $\mathrm{P}_x (a;B) = 0$），则这个新的变量满足第 $1$ 节中所有的要求。

此外，如果概率密度 $f^{(x)}$ 和 $f^{(x)}_B (a)$ 存在，且 $f^{(x)}(a) > 0$，则公式 $(3)$ 又可以写成
$$
\tag{4}
\mathrm{P}_x (a;B) = \mathrm{P}(B) \frac{f^{(x)}_B(a)}{f^{(x)}(a)}
$$
此外，如果公式 $(3)$ 中的极限存在，并且概率密度 $f^{(x)}(a)$ 存在，则 $f^{(x)}_B(a)$ 存在。因此
$$
\tag{5}
\mathrm{P}(B) f^{(x)}_B(a) \le f^{(x)}(a)
$$
如果 $\mathrm{P}(B) > 0$，则由公式 $(4)$ 可得
$$
\tag{6}
f^{(x)}_B(a) = \frac{\mathrm{P}_x (a;B) f^{(x)}(a)}{\mathrm{P}(B)}
$$
当 $f^{(x)}(a) = 0$ 时，由公式 $(5)$ 可得 $f^{(x)}_B(a) = 0$ 并且此时公式 $(6)$ 依然成立。此外，如果 $X$ 的分布是连续的，可得
$$
\tag{7}
\mathrm{P}(B) = \mathrm{E} (\mathrm{P}_x(B)) = \int _{- \infin} ^{+ \infin} \mathrm{P}_x (a;B)  d F^{(x)} (a) = \int _{- \infin} ^{+ \infin} \mathrm{P}_x (a;B) f^{(x)} (a) da
$$


由公式 $(6)$ 和 $(7)$ 可得
$$
\tag{8}
f^{(x)}_B(a) = \frac{\mathrm{P}_x (a;B) f^{(x)}(a)}{\int _{- \infin} ^{+ \infin} \mathrm{P}_x (a;B) f^{(x)} (a) da}
$$
这个公式给出了连续分布的贝叶斯定理（Bayes Theorem for continuous distributions）。这个定理得以证明的前提假设如下：

- $\mathrm{P}_x (B)$ 是波莱尔可测的，且在点  $a$ 它由公式 $(3)$ 定义；
- $X$ 为连续分布；
- 在点 $a$ 处存在概率密度 $f^{(x)}_B(a)$。



### 条件数学期望

令 $u$ 为变量 $\xi$ 的任意函数，$y$ 为一个随机变量。随机变量 $\mathrm{E}_u (y)$ 可以表示为 $u$ 的函数，且对任意的 $\mathcal{E}^{(u)}$ 中的集合 $A$，满足 $\mathrm{P}^{(u)}(A) > 0$，则以下定义（如果存在）
$$
\tag{1}
\mathrm{E}_{\{ u \subset A \}} (y) = \mathrm{E}_{\{ u \subset A \}} \mathrm{E}_u (y)
$$
称为给定 $u$ 时，变量 $y$ 的条件数学期望（conditional mathematical expectation）。

如果给公式 $(1)$ 两边乘 $\mathrm{P}^{(u)}(A)$，则有
$$
\tag{2}
\int_{\{ u \sub A \}} y \mathrm{P} (dE) = \int_A \mathrm{E}_u (y) \mathrm{P}^{(u)}(dE^{(u)})
$$
相反地，由公式 $(2)$ 也可得公式 $(1)$。当 $\mathrm{P}^{(u)}(A) = 0$ 时，公式 $(1)$ 无意义，公式 $(2)$ 是显然成立的。以与第 $1$ 节中条件概率相同的方式，可以证明 $\mathrm{E}_u (y)$ 由公式 $(2)$ 唯一确定（等价情况除外）。

当 $u = a$ 时 $\mathrm{E}_u (y)$ 的值记为 $\mathrm{E}_u (a;y)$。同样需要说明的是，$\mathrm{E}_u (y)$ 和 $\mathrm{P}_u (y)$ 仅由分割 $\mathcal{U}_{u}$ 决定，所以 $\mathrm{E}_u (a;y)$ 也可以记为 $\mathrm{E}_{\mathcal{U}_{u}} (y)$。

$\mathrm{E}(y)$ 的存在性隐含在 $\mathrm{E}_u (y)$ 的定义中（令 $A = E^{(u)}$，则 $\mathrm{E}_{\{ u \subset A \}} (y) = \mathrm{E}(y)$）。

接下来证明 $\mathrm{E}(y)$ 的存在足以保证 $\mathrm{E}_u (y)$ 的存在。为此只需证明，由 Nikodym 定理（见本章第 $1$ 节），可得1）集合函数在 $\mathcal{E}^{(u)}$ 上完全可加，并且2）关于 $\mathrm{P}^{(u)} (A)$ 绝对连续。条件 $1$ 可以按与第 $1$ 节条件概率的情况几乎完全相同的方式证明。条件 $2$ （绝对连续性）包含在这一事实中：由 $Q(A) \ne 0$ 可得，$\mathrm{P}^{(u)} (A) > 0$。如果假定 $\mathrm{P}^{(u)} (A) = \mathrm{P} \{ u \sub A \} = 0$，则显然有
$$
Q(A) = \int_{\{ u \sub A \}} y \mathrm{P} (dE) = 0
$$
由此第二个条件得到满足。

如果在公式 $(1)$ 中令 $A = E^{(u)}$，则有
$$
\tag{3}
\mathrm{E} (y) = \mathrm{E}  \mathrm{E}_u (y)
$$
进一步可以证明
$$
\tag{4}
\mathrm{E}_u (ay + bz) = a \mathrm{E}_u (y) + b \mathrm{E}_u (z)
$$
其中 $a$ 和 $b$ 为任意常数（证明留给读者）。

如果 $u$ 和 $v$ 是基本事件 $\xi$ 的两个函数，则二元组 $(u, v)$ 可以总是被当作 $\xi$ 的函数。于是有以下重要等式成立
$$
\tag{5}
\mathrm{E}_u \mathrm{E}_{(u, v)} (y) = \mathrm{E}_u (y)
$$
证明如下：$\mathrm{E}_u (y)$ 的定义如下：
$$
\mathrm{E}_{\{ u \subset A \}} (y) = \mathrm{E}_{\{ u \subset A \}} \mathrm{E}_u (y)
$$
因此必须证明 $\mathrm{E}_u \mathrm{E}_{(u, v)} (y) $ 满足如下关系：
$$
\tag{6}
\mathrm{E}_{\{ u \subset A \}} (y) = \mathrm{E}_{\{ u \subset A \}} \mathrm{E}_u \mathrm{E}_{(u, v)} (y)
$$
由 $\mathrm{E}_{(u, v)} (y)$ 的定义可知
$$
\tag{7}
\mathrm{E}_{\{ u \subset A \}} (y) = \mathrm{E}_{\{ u \sub A \}}  \mathrm{E}_{(u, v)} (y)
$$
由 $\mathrm{E}_u \mathrm{E}_{(u, v)} (y)$ 的定义可知
$$
\tag{8}
\mathrm{E}_{\{ u \sub A \}}  \mathrm{E}_{(u, v)} (y) = \mathrm{E}_{\{ u \subset A \}} \mathrm{E}_u \mathrm{E}_{(u, v)} (y)
$$
由公式 $(7)$ 和公式 $(8)$ 可证明公式 $(6)$，由此证明公式 $(5)$。



如果令 $y = \mathrm{P}_u (B)$，在集合 $B$ 上 $y = 1$，在集合 $B$ 外 $y = 0$，则
$$
\mathrm{E}_u (y) = \mathrm{P}_u (B) \\
\mathrm{E}_{(u, v)} (y) = \mathrm{P}_{(u, v)} (B)
$$
此时由公式 $(5)$ 可得
$$
\tag{9}
\mathrm{E}_u \mathrm{P}_{(u, v)} (B) = \mathrm{P}_u (B)
$$
条件数学期望 $\mathrm{E}_u (y)$ 也可以直接通过对应的条件概率的方式定义。为此考虑如下和式
$$
\tag{10}
S_{\lambda} (u) = \sum ^{k = + \infin} _{k = - \infin} k \lambda \mathrm{P}_u \{ k \lambda \le y < (k + 1) \lambda \} = \sum_k \mathrm{P}_k
$$
如果 $\mathrm{E} (y)$ 存在，则级数 $(10)$ 几乎必定（almost certainly）[^*]是收敛的。由第 $1$ 节的公式 $(3)$ 可知
$$
\mathrm{E} |R_k| = |k \lambda| \mathrm{P} \{ k \lambda \le y < (k + 1) \lambda \}
$$
以及下面级数的收敛性
$$
\sum ^{k = + \infin} _{k = - \infin} |k \lambda| \mathrm{P} \{ k \lambda \le y < (k + 1) \lambda \} = \sum_k \mathrm{E} |R_k|
$$
是 $\mathrm{E}(y)$ 存在的必要条件（见第四章，第 $1$ 节）。由这一收敛性可得级数 $(10)$ 几乎必定收敛（见第四章，第 $2$ 节，性质 V）。可以进一步证明，正如勒贝格积分理论说明的那样，由级数 $(10)$ 在当 $\lambda$ 取一些值时收敛可推得，它对所有的 $\lambda$ 都收敛；当级数 $(10)$ 收敛时，在 $\lambda \rightarrow 0$ 时[^5.3] $S_{\lambda} (u)$ 趋向于一个确定的极限，由此可以定义
$$
\tag{11}
\mathrm{E}_u (y) = \lim _{\lambda \rightarrow 0} S_{\lambda} (u)
$$
为证明公式 $(11)$ 定义的条件期望 $\mathrm{E}_u (y)$ 满足以上的种种条件，仅需证明它满足公式 $(1)$：
$$
\mathrm{E}_{\{ u \subset A \}} \mathrm{E}_u (y) = \lim _{\lambda \rightarrow 0} \mathrm{E}_{\{ u \subset A \}} S_{\lambda} (u) = \lim _{\lambda \rightarrow 0} \sum ^{k = + \infin} _{k = - \infin} k \lambda \mathrm{P}_{\{ u \sub A \}} \{ k \lambda \le y < (k + 1) \lambda \} = \mathrm{E}_{\{ u \subset A \}} (y)
$$
以上计算中，数学期望符号和积分符号可交换，因为当 $\lambda \rightarrow 0$ 时 $S_{\lambda} (u)$ 一致收敛（converges uniformly）于 $\mathrm{E}_u (y)$ （由第 $2$ 节数学期望的性质 V 可知）。数学期望符号和积分符号可交换的另一个原因是，以下级数是收敛的（数学期望性质 V 的直接结论）：
$$
\sum ^{k = + \infin} _{k = - \infin} \mathrm{E} _{\{ u \sub A \}} \{ |k \lambda | \mathrm{P}_u [ k \lambda \le y < (k + 1) \lambda ] \} = \sum ^{k = + \infin} _{k = - \infin} |k \lambda| \mathrm{P}_{\{ u \sub A \}} [ k \lambda \le y < (k + 1) \lambda ]
$$
公式 $(11)$ 的等效的另一种写法是
$$
\tag{12}
\mathrm{E}_u (y) = \int_E y \mathrm{P} (dE)
$$
此处需要说明，在第四章第 $1$ 节所述内容的意义下，公式 $(12)$ 并不是积分，所以它仅仅是一个符号化（symbolic）的表达。

如果 $x$ 是个随机变量，则称 $x$ 和 $a$ 的函数
$$
F^{(y)} _x (a) = \mathrm{P} _x (y < a)
$$
为 $y$ 对于已知 $x$ 的条件分布函数（conditional distribution function of y for known x）。

$F^{(y)} _x (a)$ 几乎对所有的 $a$ 都有定义。如果 $a < b$，则以下不等关系几乎必定成立
$$
F^{(y)} _x (a) \le F^{(y)} _x (b)
$$
 由公式 $(10)$ 和公式 $(11)$ 可得[^5.4]以下公式几乎必然成立
$$
\tag{13}
\mathrm{E}_x (y) = \lim _{\lambda \rightarrow 0} \sum ^{k = + \infin} _{k = - \infin} k \lambda [F^{(y)} _x ((k + 1) \lambda) - F^{(y)} _x (k  \lambda)]
$$
这一事实可由以下公式作一符号化的表达
$$
\tag{14}
\mathrm{E}_x (y) = \int ^{+ \infin} _{- \infin} a d F^{(y)} _x(a)
$$
由新获得的数学期望的定义（公式 $(10)$ 和公式 $(11)$），很容易证明，对任意实函数 $u$
$$
\tag{15}
\mathrm{E}_u [f(u)y] = f(u) \mathrm{E}_u(y)
$$


[^$]: 以下公式，原文等式左边为 $\mathrm{P} (B u^{-1}(A_n))$，我认为多了个 $n$。
[^5.1]: O. NIKODYM, Sur une généralisation des intégrales de M. J. Ra don, Fund. Math. v. 15, 1930 p. 168 (Theorem III).

[^5.2]: Lebesgue, l. c., 1928, pp. 301-302.
[^*]: We use almost certainly interchangeably with almost surely.
[^5.3]: 这种情况下我们仅考虑 $\lambda$ 的可数序列的值（a Countable sequence of values），这样对于所有的这些 $\lambda$，所有的概率 $\mathrm{P}_u \{ k \lambda \le y < (k + 1) \lambda \}$ 就都有定义了。
[^5.4]: Cf. footnote 3.

