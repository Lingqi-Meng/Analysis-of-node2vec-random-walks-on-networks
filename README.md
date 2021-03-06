# Analysis of node2vec random walks on networks

## Spectral gap for empirical networks

Select `Spectral gap analysis.ipynb` to evaluate and plot the spectral gap for the node2vec random walks on empirical networks. The vole network is used in the cell [2].

* One can download the data set from [Network Repository](http://networkrepository.com/). To save the readers' time, we present the hyperlinks for the data used in Fig. 2 in our [main text](https://arxiv.org/abs/2006.04904#:~:text=Algorithm%20node2vec%20employs%20biased%20random,label%20classification%20and%20link%20prediction.&text=The%20node2vec%20random%20walk%20is%20a%20second%2Dorder%20Markov%20chain.):

[Vole](http://networkrepository.com/mammalia-voles-bhp-trapping-55.php), [Dolphin](http://networkrepository.com/dolphins.php), [Enron](http://networkrepository.com/email-enron-only.php), [Jazz](http://networkrepository.com/jazz.php), [Coauthorship](http://networkrepository.com/ca-netscience.php), [Email](http://networkrepository.com/email-univ.php)

* If you need to consider a different network data set (other than the [Vole](http://networkrepository.com/mammalia-voles-bhp-trapping-55.php) network), you can

Step 1. Download the empirical data set from the hyperlink above or some other sources.

Step 2. Replace the code in the cell [2] by your target data set. 

Step 3. Restart the kernel in Jupyter notebook.

![Spectral gap for empirical networks](https://github.com/Lingqi-Meng/Analysis-of-node2vec-random-walks-on-networks/blob/master/images/image1.png)


## Spectral gap for extended ring networks

Select `Extended ring network.ipynb` to evaluate and plot the spectral gap for the node2vec random walks on extended ring networks. You can change the number of nodes in the extended ring network by changing `size` in cell [3]. The number of nodes in the example code is 100.

![Spectral gap for extended ring networks](https://github.com/Lingqi-Meng/Analysis-of-node2vec-random-walks-on-networks/blob/master/images/image2.png)

## Spectral gap for two-layer extended ring networks

Select `Two layer extended ring network.ipynb` to evaluate and plot the spectral gap for the node2vec random walks on two-layer extended ring networks. You can change the number of nodes in mono-layer $N^\prime$ and the weight $w$ in the two-layer extended ring networks. **Note that the variable `size` in cell [3] is the same as $N^\prime$ in Fig. 6 in our paper, NOT $N$.** The number of nodes in mono-layer in our example code is 100, and the weight is 1.

![Spectral gap for two-layer extended ring networks](https://github.com/Lingqi-Meng/Analysis-of-node2vec-random-walks-on-networks/blob/master/images/image3.png)

## Mean coalescence time evaluation

Select `Mean coalescence time.ipynb` to evaluate and plot the mean coalescence time on two-clique networks. You can change the initial conditions, clique size, and weight of the bridge by changing `p`, `size`, and `weight` respectively. **Note that the variable `size` in cell [3] is the same as $N/2$ in Fig.9 in our paper, NOT $N$.** The initial condition is in the example code is the uniformly random condition. The clique size is 100, i.e., N=200, and weight $w=1$. The other two initial condidtions (the two walkers are initially in the same clique or opposite cliques) can be found at the end of the comments in cell [2].

![Mean coalescence time](https://github.com/Lingqi-Meng/Analysis-of-node2vec-random-walks-on-networks/blob/master/images/image4.png)

## Dependence of the relaxation speed on the second largest eigenvalue of T

Please run `Relaxation time.ipynb` to see the numerical result. If you need to consider a different network other than the vole network, change the code in cells [2] and [6]. The instruction is the same as the one in ``Spectral gap for empirical networks``.
