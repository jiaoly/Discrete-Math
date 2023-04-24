<head>
    <script src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
    <script type="text/x-mathjax-config">
        MathJax.Hub.Config({
            tex2jax: {
            skipTags: ['script', 'noscript', 'style', 'textarea', 'pre'],
            inlineMath: [['$','$']]
            }
        });
    </script>
</head>

### Markov Decision Process

![RL-process](https://raw.githubusercontent.com/jiaoly/RL/main/Pictures/RL.png)

#### Bellman 

'''
\begin{align} U(s_0\,s_1\,s_2\,\cdots) &= \sum_{t=0}^{\infty}{\gamma^tR(s_t)} \quad 0\le\gamma<1 \\    &\le \sum_{t=0}^{\infty }{\gamma^tR_{max}} = \frac{R_{max}}{1-\gamma}    \end{align}
'''


### Model-based & Model-free

<a href="/Pictures/RL.png" download>


### Policy-based methods

#### Basic

#### REINFORCE


### Value-based methods

Advantage: More data efficiency than policy-based RL

Disadvantages: have difficulties in high dimensions/ continuous action space

#### Q-learning

#### SARSA

#### DQN (continuous inputs)





### On-Policy & Off-Policy

#### Importance sampling

#### Proximal Policy Optimization

### 


















#### 稳定性 Stability

对于传递函数$G(s)=C(sI-A)^{-1}+D$，$(sI-A)^{-1} = \frac{(sI-A)^{* }}{|sI-A|} $，其分母对应转移矩阵$A$的特征值，即传递函数极点。
对0输入系统，其稳定性判据为：**A的特征值的实部都在复平面左半平面**，对应极点对稳定性的影响。

#### 可控性 Controllability

可控性判据：**可控性矩阵$Co = [B\quad AB\quad A^{2}B\quad ……\quad A^{n-1}B]$满秩。** 由n阶系统的线性迭代形式推导，$  x_n = [B\quad AB\quad A^{2}B\quad … \quad A^{n-1}B] [ u_0\quad u_1\quad u_2 \quad… \quad u_{n-1}]^T $。即若使输入$u$有唯一解则转移矩阵必满秩。

``` 
rank(ctro(A, B))
```

#### 可稳定性 Stabilizability

存在状态负反馈使得系统稳定，判据：**任意实部大于0的A的特征值$\lambda$，矩阵$[A-\lambda I,\;B]$行满秩。**

#### 可观性 Observability




#### 可检测性：Detectablility





You can use the [editor on GitHub](https://github.com/jiaoly/jiao.github.io/edit/gh-pages/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.
This sentence uses delimiters to show math inline: $\sqrt{3x-1}+(1+x)^2$

$$\sqrt{3x-1}+(1+x)^2$$


### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List
- 
This sentence uses $ delimiters to show math inline: $\sqrt{3x-1}+(1+x)^2$


1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [Basic writing and formatting syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/jiaoly/jiao.github.io/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
