# Patch-Mixing Contrastive Regularization for Few-Label Semi-Supervised Learning

# Introduction

Recently, consistency regularization has become a fundamental component in semi-supervised learning, which tries to make the network's predictions on unlabeled data to be invariant to perturbations. However, its performance decreases drastically when there are scarce labels, e.g., $2$ labels per category. In this paper, we analyze the semantic bias problem in consistency regularization for semi-supervised learning and find that this problem stems from imposing consistency regularization on some semantically biased positive sample pairs derived from indispensable data augmentation. Based on the above analysis, we propose a patch-mixing contrastive regularization approach called $p$-Mix, for semi-supervised learning with scarce labels. In $p$-Mix, the magnitude of semantic bias is estimated by weighting augmented samples in the embedding space. Specifically, the samples are mixed in both sample space and embedding space respectively, to construct more reliable and task-relevant positive sample pairs. Then, a patch-mixing contrastive objective is designed to indicate the magnitude of semantic bias by utilizing a mixed embedding weighted by virtual soft labels. Extensive experiments were conducted, demonstrating that $p$-Mix significantly outperforms current state-of-the-art approaches. Especially, $p$-Mix achieves an accuracy of $91.95\%$ on the CIFAR-10 benchmark with only $2$ labels available for each category, which exceeds the second-best method ICL-SSL by $3.22\%$. 

<img src="./overall.png" alt="p-Mix" width="1000px" />

# TODO

The corresponding code is being collated and will be released soon.

# Citations
```
@article{pmix,
    title={Patch-Mixing Contrastive Regularization for Few-Label Semi-Supervised Learning},
    author={Xiaochang Hu, Xin Xu, Yujun Zeng and Xihong Yang},
    journal={IEEE Transactions on Artificial Intelligence}
    year={2023},
}
```
