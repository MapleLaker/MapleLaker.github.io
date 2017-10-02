---
layout:     post
title:      Merkle Tree
date:       2017-10-02
author:     Maple
header-img: img/post-bg-re-vs-ng2.jpg
catalog: true
tags:
    - tech
---

## List

Merkle Tree, 需要分3个层次，逐步去讲解。Merkle Tree 是Hash List概念上的演进。

![image](https://github.com/MapleLaker/MapleLaker.github.io/blob/master/img/bt-merkletree-intro.png?raw=true)


实际运算中，Hash运算种类非常多。位数越多，安全系统越高。理论上来说，位数决定了可枚举的空间，但是样本空间是无限的。

![image](https://github.com/MapleLaker/MapleLaker.github.io/blob/master/img/bt-hash-alg.png?raw=true)


Hash的使用场景比较多，不同的场景有不同的叫法。

![image](https://github.com/MapleLaker/MapleLaker.github.io/blob/master/img/bit-hash-usage.png?raw=true)

我们从数据完整性校验的角度，去演化Merkle Tree的诞生。
当我们下载某一个文件的时候，通过Hash数值计算，验证文件的数据完整性。
当我们从不同的不可信的机器去下载数据文件的时候，文件被分成了小块，我们需要单独的对每个块文件进行校验。在下载文件之前，我们首先需要下载Hash List.
这样我们就可以放心的去下载每一个文件块。那么如何保证Hash List没有损坏呢？我们需要一个 Root Hash.这样，我们只要下载root hash一个数值，就可以放心的从各个节点去下载文件了。

![image](https://github.com/MapleLaker/MapleLaker.github.io/blob/master/img/bit-hash-usage.-roothash.png?raw=true)

Merkle Tree做了改进，2-2 Hash,直到 Root Hash. 它的优势在于，可以选取单独的分支，单独的做检验。

![image](https://github.com/MapleLaker/MapleLaker.github.io/blob/master/img/bit-hash-usage-merkleroot.png?raw=true)








