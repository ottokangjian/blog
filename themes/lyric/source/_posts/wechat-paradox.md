---
title: 微信的社交推荐悖论与迷思
date: 2017-01-27 19:50:40
tags: ["Tech", "科技", "WeChat", "微信", "Social", "社交"]
---


2017 微信公开课 Pro 上，在明确不会提供小程序分发渠道后，小龙再一次对机器推荐和社交推荐表达了观点：

> 系统不会给你推荐一些你没有接触过的东西，系统只会强化你接触过的信息，并且不断地去学习你的历史，往你的历史方面继续推荐，但是你的朋友可能在朋友圈里面说，某一部电影很好看，那你会因为你的朋友去看了这部电影而去看这部电影，机器是无法理解这一点的

小龙曾多次提到类似的观点，并且在产品策略上身体力行——这是微信厉害的地方，别人觉得正常的实现路径，微信可以拒绝，当然它有资格拒绝。

早在 2012 年，微信“添加朋友”页面有一个公众号搜索，这个页面至今依然保留着当年的模样：一片空白，仅有一个搜索功能。持久的决心，尤其是与常人相异表现且获得成功后，更容易受人尊敬。

当然，他也说过“我所说的都是错的”。

<!-- more -->

---

## 机器推荐更差？

机器推荐并不是“只会强化你接触过的信息”。虽然我们总在诟病X宝：“为什么我买了相机还要给我推荐同款相机（而且价格更低，太恶劣太可恨）”，但事实上推荐算法中有一种称为“协同过滤（Collaborative filtering）”的方法：

> 利用社交网络中的社群经验来推荐用户感兴趣的信息。这个信息可能你接触过，可能你没有接触过，但一定是基于你的社交行为和社交关系来推荐的。

比如说，你的朋友可能在朋友圈里面说，某一部电影很好看，那你在阅读公众号时可能会看到微票儿对这部电影的推荐。

所以，机器推荐并不是更差，而是表现在另两个方面：更平庸和更有效率。

**更平庸**

我们对批量生产的工业产品的认知往往都是“平庸”。机器学习也是一样。向我推荐同一部电影，我的朋友的推荐效果肯定优于机器推荐。因为我朋友的推荐中附带了高信任值，这种信任建立在我们的友谊之上；而机器不是我的朋友，我甚至感觉不到它的人性。

**更有效率**

机器的算法并没有改变推荐的本质，只是加速了他们。就像加速了一个函数的收敛。很多计算机技术都没有改变本质，而只是加速事物的进程。有的时候这种加速进程很有意义：比如把一个产品形态的生命周期加速，缩短到盈利窗口内；而有的时候，比如对于一个社交产品，讲究效率并不一定是好事。

值得一提的是，平庸和有效率是两个中性的描述，可以用来叙述好事，也可以用来描述坏事。

## 社交推荐更好？

小龙讨厌机器推荐，喜欢社交推荐；我们对今日头条口诛笔伐，对社交推荐赞誉有加。

但问题是，社交的主体是人。如果人的视野和品味都堪忧，那么就是他们训练了今日头条给他们反馈的垃圾。这样的人在社交场合的推荐真的对胃口吗？听上去就不合逻辑，所以实际情况是这样：尽管相当优质的内容出现在了公众号中，但同时，体系内也大量充斥着虚假、无用、有害的信息，微信已经成为新的暗网，既得利益者在这里尽情收割着用户。

如果说今日头条是机器在给用户喂垃圾食物，那么公众号就是人们互相喂垃圾食物，而且大家都吃得很开心。

当然了，对此有一个解释：“如果用户觉得对胃口，那么也就没问题”，我可以称之为“产品中立论”。既然我们不认同今日头条和快播的技术中立论，那么也不应认同产品中立论。

我非常好奇，作为神，为世界制订了规则，而世界演化的方向和结果都不太喜欢，他有什么感想。

## 愿与愚昧的战争终将有胜利的一天

阿西莫夫有一部小说我非常喜欢：《神们自己》。小说标题出自德国剧作家席勒描写圣女贞德的悲剧“Die Jungfrau von Orleans”：

> 面对愚昧，神们自己也缄口不言。
> Against stupidity, the gods themselves contend in vain.
> -- 席勒

和小说中一样，我们中的大部分人既不关心科技的进步，也不关心文明变革，没有基本的审美；仅仅关心自己的生活是否过的安逸。小说中的人们尚可求助于神（虽然最终也无济于事），我们又能向谁求助呢？

前段日子和朋友聊天，他的一个观点很有意思：如果交通规则是为了约束人而存在，那么自动驾驶普及后，很多交通基础设施也就失去作用。类似地，如果有些游戏规则是为了约束人而存在，那么 AI 掌权后，这些规则也就失去了意义。

也许向 BetaCat 求助是最后的希望。

![betacat](/wechat-paradox/betacat-1.png)
