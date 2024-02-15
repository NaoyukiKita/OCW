# Chapter 2 Background

## 2.1 Data Representation

### 2.1.1 Domain Representation

**予備的な定義**

**定義2.1 (Topology)**
集合$\mathbb{X}$とその部分集合族$T$に対し, $T$が$\mathbb{X}$上の**位相**または**開集合系**であるとは, $T$が以下の要件を満たすと言うことである:
- 空集合$\Phi$と集合$\mathbb{X}$は$T$に含まれる: $\Phi \in T, \mathbb{X} \in T$
- $T$に属する任意の部分集合の和は$T$に含まれる: ${\lbrace O_i \rbrace}_{i \in I} \subseteq T \Rightarrow \bigcup_{i \in I} O_i \in T$
- $T$に属する有限個の部分集合の積は$T$に含まれる: ${\lbrace O_i \rbrace}_{i = 1}^{N} \subseteq T \Rightarrow \bigcup_{i = 1}^{N} O_i \in T$

後述の通り, ここで, $T$に属する任意の部分集合の積は$T$に含まれるとは限らないことに注意.

**定義2.2 (Topological Space)**
位相$T$が定義される集合$\mathbb{X}$を位相空間と言う.
- 例えば, 実数空間$\mathbb{R}$は位相空間である.

**定義2.3 (Open Set)**
位相空間$\mathbb{X}$の部分集合$\mathbb{A} \subset \mathbb{X}$について, $\mathbb{A}$が$T$に属するとき, $\mathbb{A}$を開集合と言う.

**定義2.4 (Closed Set)**
位相空間$\mathbb{X}$の部分集合$\mathbb{B} \subset \mathbb{X}$について, 補集合$\mathbb{X} - \mathbb{B}$が開集合であるとき, $\mathbb{B}$を閉集合と言う.

直感的には, 開集合とは境界線を持たない位相空間の部分集合と考えて良い. 簡単な例として, 実数空間$\mathbb{R}$上の開集合, 閉集合を考える:
- 開区間$(0, 1)$は開集合である.
- 開区間の和$(-\infty, 1) \cap (2, 3)$は開集合である(ちなみに, これは開区間とは言えない).
- 閉区間$[0, 1]$や閉区間の和$[0, 1] \cap [2, 3]$は閉集合である.

位相空間$T$に属する任意の部分集合の積は$T$に含まれるとは限らない. 上の例で言えば, $n$に対して定義できる$\mathbb{R}$上の開集合$O_n = (-1/n. 1/n)$を考えたとき, $\bigcap_{n = 1}^{\infty} O_n$は一点集合$\lbrace 0\rbrace$となり, これは開集合ではない.