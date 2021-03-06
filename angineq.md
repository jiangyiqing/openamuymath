<script 
  src="https://cdn.bootcss.com/mathjax/2.7.5/MathJax.js?config=TeX-MML-AM_CHTML">
</script>
# 逆向递推法证明几何均值小于算术均值
#### 引言
这个证明方法来自奥古斯丁·柯西的Cours d'Analyse。\\
之前引入基本不等式时，老师表示这东西的证明“比较麻烦”，故没有现场演示。\\
在4月19日下午，华师大老师引入了这个证明方法。全班24人中，不到10人仔细看完并理解了这个证明。\\
作为逆向递推法的第一道例题，配合四月十九日危机，严重地损害了阿姆伊人的自信心。\\
（直到我们知道是柯西给出之前，我都以为这估计是某个不知名的印度或中世纪欧洲数学家证明的。）\\
这是阿姆伊现存唯一较为完整的逆向递推法例题记录\\
——4月19日23：53（+8），阿姆伊成员0x21(Καππα)

---

$$
证明:\\
\frac{x_1+x_2+x_3+ ...+x_n}{2} \geq \sqrt[n]{x_1 x_2 x_3 ... x_n}\\
(当且仅当x_1 = x_2 = x_3 = .... =x_n时，等号成立。)
$$

---

### 证明如下：
$$1':当x_1 = x_2 = x_3 = .... =x_n时，\\左边= \frac{nx_1}{n} = x_1\\右边= \sqrt[n]{x_1^n} = x_1\\所以其算术均值等于几何均值。原命题成立。\\
//到这步为止很多人都能想到，还行。\\
2':当x_i (i = 1,2,3....n) 不全相等时，\\
若n=2，\\
(\frac{x_1+x_2}{2})^2 - (\sqrt{x_1x_2})^2 = \frac{1}{4} \cdot (x_1^2 - 2x_1x_2 + x_2^2) = (x_1 - x_2)^2 > 0\\
\therefore \frac{x_1+x_2}{2} > \sqrt{x_1x_2}\\
//基本不等式，易证。(好像这也是几何均值最常用的情况（？？？）)\\
若n=2^m (m \in \mathbb{N}^*)\\
最基本的情况m=1，n=2，刚刚已经证明过了。\\
现在，假设对于m=k成立，证明对于m=k+1也成立：\\
设m=k时，原命题成立\\
<=> \frac{x_1+x_2+x_3+...+x_{2^k}}{2^k} \geq \sqrt[2^k]{x_1x_2x_3...x_{2^k}}\\
=> \frac{x_1+x_2+x_3+...+x_{2^k}+x_{2^{k+1}}}{2^{k+1}} \geq \sqrt[2^{k+1}]{x_1x_2x_3...x_{2^k}x_{2^{k+1}}}\\
//由m=1得：\\
\frac{
        1
    }{
        2
        }
        (\frac{
            x_1 + x_2 + x_3 + ... + x_{2^k}
            }{
                2^k
            }
        +\frac{
            x_{2^k+1} + x_{2^k+2} + x_{2^k+3} + ... + x_{2^{k+1}}
            }{
                2^k
            })
\geq
\sqrt{
    \frac{
        x_1 + x_2 + x_3 + ... + x_{2^k}
    }{
        2^k
    }
    \frac{
        x_{2^k+1} + x_{2^k+2} + x_{2^k+3} + ... + x_{2^{k+1}}
    }{
        2^k
    }
}\\
当且仅当x_1=x_2=x_3=...x_{2^k}时等号成立\\
//易证的m=1居然有这么大的作用，嗯没错我就算独自做这道题40小时也想不到这一步\\
//下面一步则是由m=k得到的：\\
\geq
\sqrt{
    \sqrt[2^k]{
        x_1  x_2  x_3  ...  x_{2^k}
    }
    \sqrt[2^k]{
        x_{2^k+1}  x_{2^k+2}  x_{2^k+3}  ...  x_{2^{k+1}}
    }
}\\
当且仅当x_{2^{k}}=x_{2^{k}+1}=x_{2^{k}+2}=...x_{2^{k+1}}时等号成立\\
//假设的m=k成立，带入（1到2^k和2^k+1到2^{k+1}的项数都是2^k，因此可以使用之前的结论。\\(嗯没错我就算独自做这道题40小时也想不到这一步)^2\\
//接下来是简单的化简:\\
=
\sqrt[2^{k+1}]{
    x_1  x_2  x_3  ...  x_{2^{k+1}}
}\\
所以，形如n=2^m的情况下，原命题成立。
//至此，第一部分完成。\\我们在无穷大的地方建立了基地。是时候覆盖到全自然数了！\\4月20日00:43（+8）——阿姆伊成员0x21(Καππα)$$
$$
3'如果n不是2^k(k \in \mathbb{N}),它肯定小于2的某次方。那么不妨设2^k=m=n+1,\\
好吧，这就是说：已知，\frac{x_1+x_2+x_3+...+x_n+x_{n+1}}{n+1} \geq \sqrt[n+1]{x_1x_2x_3...x_nx_{n+1}}
=>
\frac{x_1+x_2+x_3+...+x_n}{n} \geq \sqrt[n]{x_1x_2x_3...x_n}\\
设x_{n+1} = \frac{x_1+x_2+x_3+...+x_n}{n} = \alpha\\
//既然对于任意n+1都成立，那么对于x_{n+1}等于前n个数的算术均值也是成立的。这样构造使得接下来的证明非常简单。\\
\frac{n \alpha + \alpha}{n+1} = \alpha \geq \sqrt[n+1]{x_1x_2x_3...x_n}\\
<=> \alpha^{n+1} \geq x_1x_2x_3...x_n \cdot \alpha\\
<=> \alpha^n \geq x_1x_2x_3...x_n\\
<=> \alpha \geq \sqrt[n]{x_1x_2x_3...x_n}\\
即\frac{\sum_{i=1}^nx_i}{n} \geq \sqrt[n]{\prod_{i=1}^nx_i}\\
所以原命题成立.
$$