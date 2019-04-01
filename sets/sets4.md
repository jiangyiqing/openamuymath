<script 
  src="https://cdn.bootcss.com/mathjax/2.7.5/MathJax.js?config=TeX-MML-AM_CHTML">
</script>
# 集合的运算
* 2019年4月1日
## 交集
定义：
$$\textrm{A} \cap \textrm{B} = \left \{ x|x\in\textrm{A}$$ 且 $$x\in \textrm{B} \right \} $$
* 1' $$\textrm{A} \cap \textrm{B} = \textrm{B}\cap  \textrm{A}$$
* 2' $$\textrm{A}\cap  (\textrm{B}\cap  \textrm{C} )=( \textrm{A} \cap \textrm{B})\cap  \textrm{C} = (\textrm{A}\cap  \textrm{C})\cap  \textrm{B}$$
* 3' $$\varnothing \cap \textrm{A} =\varnothing$$
#### 例题一
1':
$$\textrm{A} = \left \{ y|y=2x+1 ,x,y\in \mathbb{R} \right \} \\\textrm{B} = \left \{ y|y=-x^2+9 ,x,y\in \mathbb{R} \right \} \\\textrm{A} \cap \textrm{B} = \left (-\infty  ,9 \right ]$$
2':
$$\textrm{A} = \left \{ (x,y)|y=2x+1 ,x,y\in \mathbb{R} \right \} \\\textrm{B} = \left \{ (x,y)|y=-x^2+9 ,x,y\in \mathbb{R} \right \} \\\textrm{A} \cap \textrm{B} = \left \{ (2,5),(-4,-7) \right \}$$
## 并集
定义：
$$\textrm{A} \cap \textrm{B} = \left \{ x|x\in\textrm{A}$$ 或 $$x\in \textrm{B} \right \} $$
* 1‘ $$\textrm{A} \cup \textrm{B} = \textrm{B}\cup  \textrm{A}$$
* 2’ $$\textrm{A}\cup  (\textrm{B}\cup  \textrm{C} )=( \textrm{A} \cup \textrm{B})\cup  \textrm{C} = (\textrm{A}\cup  \textrm{C})\cup  \textrm{B}$$
* 3‘ $$\varnothing \cup  \textrm{A} =\textrm{A}$$
## 定律(结合律)
$$\textrm{A}\cap (\textrm{B}\cup \textrm{C}) = (\textrm{A}\cap \textrm{B})\cup (\textrm{A}\cap \textrm{C})\\\textrm{A}\cup (\textrm{B}\cap \textrm{C}) = (\textrm{A}\cup \textrm{B})\cap (\textrm{A}\cup \textrm{C})$$
#### 例题二
若$$\textrm{A} \cap \textrm{B} =\textrm{A}$$ 则$$\textrm{A} \subseteq \textrm{B}\\$$
若$$\textrm{A} \cup \textrm{B} =\textrm{A}$$ 则$$\textrm{A} \supseteq \textrm{B}$$
## 补集
定义：
设U为全集，$$\textrm{A} \subseteq \textrm{U}\\$$
$$\complement_U \textrm{A} = \left \{ x|x\in \textrm{U}$$ 且 $$x \notin \textrm{A}  \right \}$$
#### 例题三
$$\textrm{U} = [1,\pi )\\\textrm{A} = \left \{ x|x^2-x-2<0,x\in\textrm{U} \right \}\\\complement_UA=[2,\pi )$$
#### 例题四
设全集
## 德·摩根定律
## 练习
#### 1
#### 2
#### 3