---
title: how-to-resolve-referace-cycle
date: 2017-05-19 14:33:34
tags:
---
一方属性不可以为nil时，使用unowned
一方属性可以为nil时，使用weak
双方属性都不可以为nil时 使用
用implicit unwrapped optional伪装起来，让它还是一个optional，而另一个属性定义为unowned就好了。