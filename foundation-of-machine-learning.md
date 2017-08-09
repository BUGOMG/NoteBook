#最大似然估计估计

<font size=10 color="red">为包含m个样本的数据</font>$$\mathbb{X}=\{x_1,\cdots,x_n\}$$，由分布$$P_{data}(x;\pmb{\theta})$$产生，那么对应的似然函数为：
$$\prod_\limits{i=1}^{n}P(x_i;\pmb{\theta})=P(\mathbb{X};\pmb{\theta})$$
&emsp;&emsp;对于未知参数$$\theta$$的最大似然估计如下
$$\theta_{ML}=\arg\max_{\theta^*}\prod\limits_{i=1}^{n}P(x_i;\pmb{\theta^*})$$

另一种最大似然估计的解释，认为它是最小化训练集分布$$P_{data}(\mathbb{X};\pmb{\theta})$$与模型分布$$P_{model}(\mathbb{X};\pmb{\theta})$$之间的差异，差异使用KL散度的方式度量：
$$\begin{split}
   D_{KL} &= \frac{1}{n}\sum\limits_{i=1}^{n}\log P_{data}(x_i;\pmb{\theta})-\log P_{model}(x_i;\pmb{\theta})\\
          &= E_{x\sim P_{data}}\left[ \log P_{data}(\mathbb{X;\pmb{\theta}}) - \log P_{model} (\mathbb{X;\pmb{\theta}})\right]
\end{split}$$
其中第一项是常数，所以可以去掉最后为：$$-E_{x\sim P_{data}} \log P_{model} (\mathbb{X;\pmb{\theta}})$$
