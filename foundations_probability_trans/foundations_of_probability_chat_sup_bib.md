# 关于补充参考文献的说明

概率论的测度论方法的奠基性著作是 A. N. 柯尔莫哥洛夫的《Grundbegriffe der Wahrscheinlichkeitsrechnung》（《概率论基本概念》德文版本），本文是其英文翻译版本。可以毫不夸张地说，在过去的二十三年间，大部分概率论研究都受到这一方法的影响，而且柯尔莫哥洛夫提出的公理体系已被概率论与统计学界学者公认为正确的理论基础。

柯尔莫哥洛夫《Grundbegriffe der Wahrscheinlichkeitsrechnung》的出版开启了概率论及其研究方法的新纪元，基于科尔莫戈洛夫提出的基本概念所产生的研究成果非常丰富。在准备科尔莫戈洛夫专著英文译本第二版的过程中，我们认为有必要提供一份能反映概率论研究现状与方向的书目。

近几年出版了许多优秀的（概率论相关的）书籍，其中最具代表性的三部分别是Doob [12]， Feller [17]，和 Loève [54]的作品。以下是涉及概率论通论及概率专题研究的其他著作：[2]，[3]，[6]，[7]，[9]，[19]，[23]，[26]，[27]，[28]，[34]，[39]，[41]，[42]，[47]，[49]，[50]，[67]，[70]，[72]。鉴于这些著作已收录大量文献索引，此处将重点列出近年已发表的研究论文和即将发表的论文。

柯尔莫哥洛夫建立的模型可简要表述如下：在所有包含随机因素的情况中（例如，实验、观测等），都有一个与之关联的概率空间或三元组（$\Omega$，$\xi$，$p$），其中 $\Omega$ 是抽象空间（基本事件的空间），$\xi$ 是 $\Omega$ 的子集（事件的集合）的 $\sigma$ 代数，$p(E)$ 是根据 $E$、$\epsilon$、$\xi$ 定义的一个测度（事件 $E$ 的概率），并且满足 $p(\Omega) = 1$。Loś [56] 最近研究了柯尔莫哥洛夫的模型，他尝试使用抽象代数和集合的 $\sigma$ 代数来代替传统意义上的代数与 $\sigma$ 代数。柯尔莫哥洛夫 [44] 也尝试过在概率论中使用度量布尔代数（metric Boolean algebras）。

有许多问题，尤其是在理论物理领域，无法纳入柯尔莫哥洛夫理论，其原因在于这些问题涉及无界测度（unbounded measures）。Rényi [68] 建立了一种广义的公理化概率理论（该理论将柯尔莫哥洛夫的理论作为一个特例），这一理论允许无界测度的存在。这一理论的基础概念是事件的条件概率。Császár [10] 研究了 Rényi 的理论中的条件概率空间的测度论结构。

在另一个方向上，很多作者指出柯尔莫哥洛夫的理论过于宽泛。Gnedenko 和 柯尔莫哥洛夫 [27] 提出了一种称为**完美概率空间**（perfect probability space）的限制性更强的概念。完美概率空间是这样一个三元组 $(\Omega, \xi, p)$，满足对任意实值 $\xi$ 可测函数 $g$ 和任意线性集 $B$，若集合 $\{ \omega : g(\omega) \in B \} \in \xi$，则存在一个波莱尔集 $D \subseteq B$，满足 $\mathrm{P} \{ \omega : g(\omega) \in D \} = \mathrm{P} \{ \omega : g(\omega) \in B \}$。最近，Blackwell [5] 提出了一个比完美概率空间更严格的概念—— Lisin 空间。Lusin 空间是一个满足如下条件的数对 $(\Omega, \xi)$：

- $\xi$ 是可分的；
- $\Omega$ 上的每一个实值 $\xi$ 可测函数 $g$ 的值域，是一个解析集（analytic set）。

显然，如果 $(\Omega, \xi, p)$ 是一个 Lusin 空间，并且 $p$ 是 $\xi$ 上的任意概率测度，则 $(\Omega, \xi, p)$ 是一个完美概率空间。

在第六章第 $1$ 节，柯尔莫哥洛夫给出了马尔可夫链的定义。近些年里马尔可夫链理论和马尔可夫过程是概率领域最活跃的研究领域之一。文献 [17] 提供了该理论的一份精彩的导论。其他参考文献包括 [2]， [3]， [6]， [12]， [19]， [23]， [26]， [34]， [39]， [50]， [54]， [67]， [70]， [72]。还有两篇值得关注的论文：Harris 和 Robbins [29] 关于马尔可夫链的各态便利性理论（ergodic theory） ，以及Chung [8] 的关于状态数可数情况下的连续参数过程理论。Chung 提出的理论统一并扩展了 Doob （参考文献 [12]）和 Lévy [51],，[52]， [53] 的研究成果。

一些概率论研究工作者正在利用半群理论[30] 来研究马尔可夫过程及其结构性质 [63]。在这一方法主要是Yosida [80] 提出的，由一个 Banach 空间到自身的单参数（离散或连续）算子半群定义马尔可夫过程。Hille [32] 和 Kato [38] 使用半群方法对柯尔莫哥洛夫微分方程做积分，Kendall 和 Reuter [40] 研究了该理论中出现的一些病态案例。Feller [18] 和 Hille [31] 研究了连续情况下的抛物型微分方程（parabolic differential equations）。Doob [13] 使用半群理论中的鞅论（martingale theory）研究一维扩散过程。Hunt [33] 研究了李群（Lie groups）上的半群（概率）测度。

最近的研究论文致力于使用更抽象的方式研究概率。这些研究探讨具有代数结构的拓扑空间中的随机变量。文献 [14]，[21]，[22]，[58]，[59]，[61] 研究了与巴拿赫空间（Banach space）中的随机变量有关的问题，文献 [4] 研究了 Orlicz 空间（广义勒贝格空间）中的类似问题。Robbins [69] 研究了任意紧致拓扑空间（compact topological group）中的随机变量。Segal [75] 研究了概率代数的结构，并且使用这一代数方法推广了柯尔莫戈洛夫关于具有任意指定联合分布的实值随机变量的存在性定理（参考第三章第 $4$ 节）。Segal [76，第三章第 $13$ 节[^*]] 还研究过非交换概率理论（non-commutative probability theory）。

Prohorov [66] 研究了定义在巴拿赫空间和其他函数空间上的概率分布的收敛性质。LeCam [48] 和 Parzen [64] 也研究过这些问题。

柯尔莫哥洛夫在第四章（以及文献 [12] 和 [54]）中给出了条件概率和条件数学期望的测度论定义和基本性质。使用抽象代数方法，S. T. C. Moy [60] 将条件数学期望的性质视为概率空间上所有的扩展实值可测函数（extended real-valued measurable functions）空间到自身的线性变换。在文献 [61] 中，她研究了巴拿赫空间随机变量的条件数学期望。Nakamura 和 Turamuru [62] 将数学期望视为 $C^*$ 代数的一种给定运算。Umegaki [79] 将条件数学期望作为属于具有 $W^*$ 代数的 $L_1$ 可积类（integrable class）的可测算子空间到自身的映射。Umegaki 的研究发展了非可交换概率理论。以上研究用到了 Segal [74]、Dye [15] 等学者对抽象积分理论的研究成果。其他相关研究论文包括 [1]，[16]，[36]，[45]。

Gel’fand [24] 对广义随机过程（generalized stochastic processes）的研究用到了 L. Schwartz 关于分布的理论（广义函数理论，The L. Schwartz theory of distributions） [73]。后者也被 Fortet [20] 和 Itô [35] 用来研究随机分布。

还有一些研究者致力于研究概率论中的极限定理：[27]，[42]，[47]，[49]。此外，还有必要参考下文献 [12] 和 [54]。另外还有研究论文和综述论文： [11]， [14]， [25]， [37]， [46]， [55]， [57]， [65]， [71]， [77]，[78]。



[^*]: 原文有误，第三章仅存在 $5$ 节，可能指第 $3$ 节



# 补充参考文献

[1] ALDA, V., On Conditional Expectations, Czechoslovak Math. J., Vol. 5 (1955), pp. 503–505.

[2] ARLEY, N., On the Theory of Stochastic Processes and Their Application to the Theory of Cosmic Radiation, Copenhagen, 1943.

[3] BARTLETT, M. S., An Introduction to Stochastic Processes, Cambridge, 1955.

[4] BHARUCHA-REID, A. T., On Random Elements in Orlicz Spaces, (Abstract) Bull. Amer. Math. Soc., Vol. 62 (1956). To appear.

[5] BLACKWELL, D., On a Class of Probability Spaces, Proc. Third Berkeley Symposium on Math. Statistics and Probability, Vol. 2 (1956). To appear.

[6] BLANC-LAPIERRE, A., and R. Fortet, Théorie des fonctions aléatoires, Paris, 1953.

[7] BOCHNER, S., Harmonic Analysis and the Theory of Probability, Berkeley and Los Angeles, 1955.

[8] CHUNG, K. L., Foundations of the Theory of Continuous Parameter Markov Chains, Proc. Third Berkeley Symposium on Math. Statistics and Probabiilty, Vol. 2 (1956). To appear.

[9] CRAMÉR, H., Mathematical Methods of Statistics, Princeton, 1946.

[10] CSÁSZÁR, A., Sur le structure des espace de probabilité conditionnelle, Acta Math. Acad. Sci. Hung., Vol. 6 (1955), pp. 337–361.

[11] DERMAN, C., and H. ROBBINS, The Strong Law of Large Numbers when the First Moment does not Exist, Proc. Nat. Acad. Sci. U.S.A., Vol. 41 (1955), pp.586–587.

[12] DOOB, J. L., Stochastic Processes, New York, 1953.

[13] DOOB, J. L., Martingales and One-Dimensional Diffusion, Trans. Amer. Math. Soc., Vol. 78 (1955), pp. 168–208.

[14] DOSS, S., Sur le théorème limite central pour des variables aléatoires dans espace de Banach, Publ. Inst. Statist. Univ. Paris, Vol. 3 (1954), pp. 143–148.

[15] DYE, H. A., The Radon-Nikodym Theorem for Finite Rings of Operators, Trans. Amer. Math. Soc., 72 (1952), pp. 243–280.

[16] FABIÁN, V., A Note on the Conditional Expectations, Czechoslovak Math. J., Vol. 4 (1954), pp. 187–191.

[17] FELLER, W., An Introduction to Probability Theory and Its Applications, New York, 1950.

[18] FELLER, W., Diffusion Processes in One Dimension, Trans. Amer. Math. Soc., Vol. 77 (1954), pp. 1–31.

[19] FORTET, R., Calcul des probabilités, Paris, 1950.

[20] FORTET, R., Random Distributions with an Application to Telephone Engineering, Proc. Third Berkeley Symposium on Math. Statistics and Probability, Vol. 2 (1956). To appear.

[21] FORTET, R., and E. MOURIER, Résultats complémentaires sur les éléments aléatoires prenant leurs valeurs dans un espace de Banach, Bull. Sci. Math. (2), Vol. 78 (1954), pp. 14–30.

[22] FORTET, R., and E. MOURIER, Les fonctions aléatoires comme éléments aléatoires dans les espace de Banach, Stud. Math., Vol. 15 (1955), pp. 62–79.

[23] FRECHET, M., Recherches théoriques modernes sur le calcul des probabilités. II. Méthode des fonctions arbitraires. Théorie des événements en chaine dans d’un nombre fini d’états possibles, Paris, 1938.

[24] GEL’FAND, I. M., Generalized Random Processes, Doklady Akad. Nauk SSSR (N.S.), Vol. 100 (1955), pp. 853–856. [In Russian.]

[25] GIHMAN, I. L., Some Limit Theorems for Conditional Distributions, Doklady Akad. Nauk SSSR (N.S.), Vol. 91 (1953), pp. 1003–1006. [In Russian.]

[26] GNEDENKO, B. V., Course in the Theory of Probability, Moscow-Leningrad, 1950. [In Russian.]

[27] GNEDENKO, B. V., and A. N. KOLMOGOROV, Limit Distributions for Sums of Independent Random Variables, Translated by K. L. Chung with an appendix by J. L. Doob, Cambridge, 1954.

[28] HALMOS, P. R., Measure Theory, New York, 1950.

[29] HARRIS, T. E., and H. ROBBINS, Ergodic Theory of Markov Chains Admitting an Infinite Invariant Measure, Proc. Nat. Acad. Sci. U.S.A., Vol. 39 (1953), pp. 860–864.

[30] HILLE, E., Functional Analysis and Semi-Groups, New York, 1948.

[31] HILLE, E., On the Integration Problem for Fokker-Planck’s Equation in the Theory of Stochastic Processes, Onzième congrès des math. scand. (1949), pp. 185–194.

[32] HILLE, E., On the Integration of Kolmogoroff’s Differential Equations, Proc. Nat. Acad. Sci. U.S.A., Vol. 40 (1954), pp. 20–25.

[33] HUNT, G. A., Semi-Groups of Measures on Lie Groups, Trans. Amer. Math. Soc., Vol. 81 (1956), pp. 264–293.

[34] ITÔ, K., Theory of Probability, Tokyo, 1953.

[35] ITÔ, K., Stationary Random Distributions, Mem. Coll. Sci. Univ. Kyoto, Ser. A. Math., Vol. 28 (1954), pp. 209–223.

[36] JIŘINA, M., Conditional Probabilities on Strictly Separable σ-Algebras, Czechoslovak Math. J., Vol. 4 (1954), pp. 372–380. [In Czech.]

[37] KALLIANPUR, G., On a Limit Theorem for Dependent Random Variables, Doklady Akad. Nauk SSSR (N.S.) Vol. 101 (1955), pp. 13–16. [In Russian.]

[38] KATO, T., On the Semi-Groups Generated by Kolmogoroff’s Differential Equations, J. Math. Soc. Japan, Vol. 6 (1954), pp. 1–15.

[39] KAWADA, Y., The Theory of Probabiilty, Tokyo, 1952.

[40] KENDALL, D. G., and G. E. H. REUTER, Some Pathological Markov Processes with a Denumerable Infinity of States and the Associated Semigroups of Transformations in l, Proc. Symp. on Stochastic Processes (Amsterdam), 1954. To appear.

[41] KHINTCHINE, A., Asymptotische Gesetze der Wahrscheinlichkeitsrechnung, Berlin, 1933. [Reprint, CHELSEA PUBLISHING COMPANY.]

[42] KHINTCHINE, A., Limit Laws of Sums of Independent Random Variables, Moscow-Leningrad, 1938. [In Russian.]

[43] KOLMOGOROV, A., Grundbegriffe der Wahrscheinlichkeitsrechnung, Berlin, 1933. [The present work is an English translation of this.]

[44] KOLMOGOROV, A., Algèbres de Boole métriques complètes, VI Zjazd Mat. Pols., Warsaw (1948), pp. 21–30.

[45] KOLMOGOROV, A., A Theorem on the Convergence of Conditional Mathematical Expectations and Some of Its Applications, Comptes Rendus du Premier Congrès des Mathématiciens Hongrois (1952), pp. 367–386. [In Russian and Hungarian.]

[46] KOLMOGOROV, A., Some Work of Recent Years in the Field of Limit Theorems in the Theory of Probability, Vestnik Moskov. Univ. Ser. Fiz.-Mat. Estest. Nauk, Vol. 8 (1953), pp. 29–38.

[47] KUNISAWA, K., Limit Theorems in Probability Theory, Tokyo, 1949.

[48] LECAM, L., Convergence in Distribution of Stochastic Processes, Univ. California Publ. Statistics. To appear.

[49] LEVY, P., Théorie de l’addition des variables aléatoires, Paris, 1937.

[50] LEVY, P., Processus stochastiques et mouvement Brownien, Paris, 1948.

[51] LEVY, P., Systèmes markoviens et stationnaires. Cas dénombrable, Ann. Sci. Ecole Norm. Sup., Vol. 68 (1951), pp. 327–401.

[52] LEVY, P., Complément à l’étude des processus de Markoff, Ann. Sci. Ecole Norm. Sup., Vol. 69 (1952), pp. 203–212.

[53] LEVY, P., Processus markoviens et stationnaires du cinquieme type (infinité denombrable d’états possibles, paramètre continu), C. R. Acad. Sci. Paris, Vol. 236 (1953), pp. 1630–1632.

[54] LOÈVE, M., Probability Theory, New York, 1955.

[55] LOÈVE, M., Variational Terms and the Central Limit Problem, Proc. Third Berkeley Symposium on Math. Statistics and Probability, Vol. 2 (1956). To appear.

[56] LOS, J., On the Axiomatic Treatment of Probability, Colloq Math., Vol. 3 (1955), pp.125–137.

[57] MARSAGLIA, G., Iterated Limits and the Central Limit Theorem for Dependent Variables, Proc. Amer. Math. Soc., Vol. 5 (1954), pp. 987–991.

[58] MOURIER, E., Eléments aléatoires dans un espace de Banach, Ann. Inst. H. Poincare, Vol. 13 (1953), pp. 161–244.

[59] MOURIER, E., L-Random Elements and L-Random Elements in Banach Spaces, Proc. Berkeley Symposium on Math. Statistics and Probability, Vol. 2 (1956). To appear.

[60] MOY, S. T. C., Characterizations of Conditional Expectation as a Transformation on Function Spaces, Pacific J. Math., Vol. 4 (1954), pp. 47–63.

[61] MOY, S. T. C., Conditional Expectations of Banach Space Valued Random Variables and Their Properties, (Abstract) Bull. Amer. Math. Soc., Vol. 62 (1956). To appear.

[62] NAKAMURA, M. and T. TURUMARU, Expectation in an Operator Algebra, Tôhoku Math. J., Vol. 6 (1954), pp. 182–188.

[63] NEVEU, J., Etude des semi-groups de Markoff, (Thesis) Paris, 1955.

[64] PARZEN, E., Convergence in Distribution and Fourier-Stieltjes Transforms of Random Functions, (Abstract) Ann. Math. Statistics, Vol. 26 (1955), p. 771.

[65] PARZEN, E., A Central Limit Theorem for Multilinear Stochastic Processes, (Abstract) Ann. Math. Statistics, Vol. 27 (1956), p. 206.

[66] PROHOROV, Yu. V., Probability Distributions in Functional Spaces, Uspehi Matem. Nauk (N.S.), Vol. 8 (1953), pp. 165–167. [In Russian.]

[67] RENYI, A., The Calculus of Probabilities, Budapest, 1954. [In Hungarian.]

[68] RENYI, A., On a New Axiomatic Theory of Probability, Acta Math. Acad. Sci. Hung., Vol. 6 (1955), pp. 285–335.

[69] ROBBINS, H., On the Equidistribution of Sums of Independent Random Variables, Proc. Amer. Math. Soc., Vol. 4 (1953), pp. 786–799.

[70] ROMANOVSKI, V. I., Discrete Markov Chains, Moscow-Leningrad, 1949. [In Russian.]

[71] ROSENBLATT, M., A Central Limit Theorem and a Strong Mixing Condition, Proc. Nat. Acad. Sci. U.S.A., Vol. 42 (1956), pp. 43–47.

[72] SARYMSAKOV, T. A., Elements of the Theory of Markov Processes, Moscow, 1954. [In Russian.]

[73] SCHWARTZ, L., Théorie des distributions, Paris, 1950–51.

[74] SEGAL, I. E., A Non-Commutative Extension of Abstract Integration, Ann. Math. Vol. 57 (1953), pp. 401–457.

[75] SEGAL, I. E., Abstract Probability Spaces and a Theorem of Kolmogoroff, Amer. J. Math., Vol. 76 (1954), pp. 177–181.

[76] SEGAL, I. E., A Mathematical Approach to Elementary Particles and Their Fields, University of Chicago, 1955. [Mimeographed Lecture Notes.]

[77] TAKANO, K., On Some Limit Theorems of Probability Distributions, Ann. Inst. Statist. Math., Tokyo, Vol. 6 (1954), pp. 37–113.

[78] TSURUMI, S., On the Strong Law of Large Numbers, Tôhoku Math. J., Vol. 7 (1955), pp. 166–170.

[79] UMEGAKI, H., Conditional Expectation in an Operator Algebra, Tôhoku Math. J., Vol. 6 (1954), pp. 177–181.

[80] YOSIDA, K., Operator Theoretical Treatment of the Markoff’s Process, Proc. Imp. Acad. Japan, Vol. 14 (1938), pp. 363–367.
