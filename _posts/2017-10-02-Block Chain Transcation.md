---
layout:     post
title:      Block Chain Transaction
date:       2017-10-02
author:     Maple
header-img: img/post-bg-re-vs-ng2.jpg
catalog: true
tags:
    - tech
---

## List
私钥 - 创建签名 - 也就是真正的密码
公钥 - 验证签名 - 也就是地址
签名 - 证明你拥有这个私钥，但同时不用暴露你的私钥

![image](https://github.com/MapleLaker/MapleLaker.github.io/blob/master/img/bt-yanzhengxitong.png?raw=true)

当你要花钱的时候，需要证明自己是这个公钥的真正拥有者。可以拿出信息，加上私钥，运算出签名。
![image](https://github.com/MapleLaker/MapleLaker.github.io/blob/master/img/bt-yanzhengxitong-qianming.png?raw=true)

别人拿到签名，再加上信息，就可以放到另外一个函数中，运算下，看是否和公钥相匹配。这样，不用看你的私钥，通过数学的方式，就可以验证你是否为私钥和公钥的拥有者，
![image](https://github.com/MapleLaker/MapleLaker.github.io/blob/master/img/bt-yanzhengxitong-yanzheng.png
?raw=true)




