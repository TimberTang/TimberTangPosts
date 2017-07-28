---
title: iOS 10.3 keychain 功能重大更改
date: 2017-03-10 09:43:28
tags:
---
> 如果 App 被删除，之前存储于 keychain 中的数据也会一同被清除。
如果使用了 keychain group，只要当 group 所有相关的 App 被删除时，keychain 中的数据才会被删除。

[相关消息](https://forums.developer.apple.com/message/75464)
[相关消息](https://forums.developer.apple.com/message/112523)

对keychain 和keychin group 不理解的可以看看[这篇文章](http://evgenii.com/blog/sharing-keychain-in-ios/)

# 扯一下iOS设备获取唯一设备号的历史变迁
```
iOS中获取设备唯一标示符的方法一直随版本的更新而变化。
iOS 2.0版本以后UIDevice提供一个获取设备唯一标识符的方法uniqueIdentifier，
但是好像是iOS 4还是iOS5就被苹果废弃掉了，
然后iOS6是用WiFi的mac地址来获取的，
iOS7后大家都知道了，主要是由于苹果又坑爹了，封杀mac地址，
但是推荐大家用KeyChain来保存获取到的UDID，因为APP删了再装回来，也可以从KeyChain中读取回来，
而现在 keychain 随着APP的写在而删除了. 
```

apple在保护隐私方面最近是作出了重大的修改

最后 很多人应该有句话要讲了吧