>  [git markdown参考](https://github.com/guodongxiaren/README#链接)
# 常用语法

# 公式语法
> 部分内容可参阅  [markdown插入数学公式](https://juejin.im/post/5a6721bd518825733201c4a2)

### 希腊字母

$$
\begin{array}{|c|c|c|c|c|c|c|c|}
\hline
{\alpha} & {\backslash alpha} & {\theta} & {\backslash theta} & {o} & {o} & {\upsilon} & {\backslash upsilon} \\\\
\hline
{\beta} & {\backslash beta} & {\vartheta} & {\backslash vartheta} & {\pi} & {\backslash pi} & {\phi} & {\backslash phi} \\\\
\hline
{\gamma} & {\backslash gamma} & {\iota} & {\backslash iota} & {\varpi} & {\backslash varpi} & {\varphi} & {\backslash varphi} \\\\
\hline
{\delta} & {\backslash delta} & {\kappa} & {\backslash kappa} & {\rho} & {\backslash rho} & {\chi} & {\backslash chi} \\\\
\hline
{\epsilon} & {\backslash epsilon} & {\lambda} & {\backslash lambda} & {\varrho} & {\backslash varrho} & {\psi} & {\backslash psi} \\\\
\hline
{\varepsilon} & {\backslash varepsilon} & {\mu} & {\backslash mu} & {\sigma} & {\backslash sigma} & {\omega} & {\backslash omega} \\\\
\hline
{\zeta} & {\backslash zeta} & {\nu} & {\backslash nu} & {\varsigma} & {\backslash varsigma} & {} & {} \\\\
\hline
{\eta} & {\backslash eta} & {\xi} & {\backslash xi} & {\tau} & {\backslash tau} & {} & {} \\\\
\hline
{\Gamma} & {\backslash Gamma} & {\Lambda} & {\backslash Lambda} & {\Sigma} & {\backslash Sigma} & {\Psi} & {\backslash Psi} \\\\
\hline
{\Delta} & {\backslash Delta} & {\Xi} & {\backslash Xi} & {\Upsilon} & {\backslash Upsilon} & {\Omega} & {\backslash Omega} \\\\
\hline
{\Omega} & {\backslash Omega} & {\Pi} & {\backslash Pi} & {\Phi} & {\backslash Phi} & {} & {} \\\\
\hline
\end{array}
$$
> 更多请见 [LATEX数字符号表](https://github.com/mk43/BlogResource/blob/master/LaTex/LATEX数学符号表.pdf)


作者：fitzeng
链接：https://juejin.im/post/5a6721bd518825733201c4a2
来源：掘金
著作权归作者所有。商业转载请联系作者获得授权，非商业转载请注明出处。

### 公式插入
    $$
    \sigma = D·\epsilon
    $$

$$
\sigma = D·\epsilon
$$

### 换行
使用 \\\\\\\\ 

    $$ 
    \sigma = D·\epsilon \\\\
    \epsilon_x = \frac{\partial u}{\partial x}
    $$
$$ 
\sigma = D·\epsilon \\\\
\epsilon_x = \frac{\partial u}{\partial x}
$$

### 对齐
使用 begin{align}、end{align}， &选择对齐位置

    $$ 
    \begin{align}
    \sigma &= D·\epsilon \\\\
    \epsilon_x &= \frac{\partial u}{\partial x}
    \end{align}
    $$

$$
\begin{align}
\sigma &= D·\epsilon \\\\
\epsilon_x &= \frac{\partial u}{\partial x}
\end{align}
$$

    To be continue...