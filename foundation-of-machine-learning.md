#最大似然估计估计

<font size=10>为包含m个样本的数据</font>$$\mathbb{X}=\{x_1,\cdots,x_n\}$$，由分布$$P_{data}(x;\pmb{\theta})$$产生，那么对应的似然函数为：
$$\prod_\limits{i=1}^{n}P(x_i;\pmb{\theta})=P(\mathbb{X};\pmb{\theta})$$
&emsp;&emsp;对于未知参数$$\theta$$的最大似然估计如下
$$\theta_{ML}=\arg\max_{\theta^*}\prod\limits_{i=1}^{n}P(x_i;\pmb{\theta^*})$$
