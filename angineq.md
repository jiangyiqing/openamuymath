<script 
  src="https://cdn.bootcss.com/mathjax/2.7.5/MathJax.js?config=TeX-MML-AM_CHTML">
</script>
# 逆向递推法证明几何均值小于算术均值
这个证明方法来自奥古斯丁·柯西的Cours d'Analyse。

---

$$
证明
\frac{x_1+x_2+x_3+ ...+x_n}{2} \geq \sqrt[n]{x_1 x_2 x_3 ... x_n}\\
当且仅当x_1 = x_2 = x_3 = .... =x_n时，等号成立。
$$
### 证明如下：

* 1' 
$$
当x_1 = x_2 = x_3 = .... =x_n时，\\左边= \frac{nx_1}{n} = x_1\\右边= \sqrt[n]{x^n} = x_1\\所以其算术均值等于几何均值。原命题成立。\\
$$
* 2' 
$$
当x_i (i = 1,2,3....n) 不全相等时，\\
若n=2，\\
(\frac{x_1+x_2}{2})^2 - (\sqrt{x_1x_2})^2 = frac{1}{4} \cdot (x_1^2 - 2x_1x_2 + x_2^2) = (x_1 - x_2)^2 > 0\\
\therefore \frac{x_1+x_2}{2} > \sqrt{x_1x_2}$$