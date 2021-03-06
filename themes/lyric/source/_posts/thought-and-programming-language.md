---
title: 思维与语言
date: 2012-08-15 15:09:19
tags: ["Life", "生活", "Thinking"]
---

不同语言里所包含的文化概念和分类会影响语言使用者对于现实世界的认知，也就是说不同的语言的使用者会因语言差异而产生思考方式，行为方式的不同，这叫[Sapir–Whorf 假说](http://en.wikipedia.org/wiki/Linguistic_relativity)。

<!--more-->

这个假说得到了相当多的例证，虽然因此断言语言主宰了思维不妥，但是说语言影响了思维方式没问题。

相对于我们使用的自然语言，程序设计语言有明显的局限性。对于程序设计语言(PL)来说，只要他们是图灵完备的，那么从根本上说任何 PL 在表达能力上都没有任何差异。也就是 A 语言能做的事，你使用别的语言也能做。这就是所谓“语言是浮云”说法的来源。

那么既然众生而平等，为什么还要发明那么多语言，为什么程序员总喜欢为了某种语言的优劣干嘴炮？

使用程序设计语言的目的是为了解决问题。要达到这一目标，就需要一个合适的策略，也就是算法。算法就是解决问题的思维方法，程序设计语言用于描述算法，就是描述解决问题的方法。

每种语言都有自己的特性。面对同一问题时，我们的思维方法——也就是算法——必然会对这些特性的差异呈现出某种适应性。当差异足够大时，这种适应性就演变成了多样性：我们的目标没变，但是思维方式变了。就像从武汉去重庆，可以坐飞机，也可以坐火车，还可以沿长江而上。

---

一个例子：假设现在我们需要用 Python 和 C 处理同一个字符串相关的问题。
如果使用C语言，我们很可能是以字节为单位操作比特数组；
但是如果使用 Python ，我们考虑的粒度会粗得多：以字符串为单位去利用Python的字符串操作能力来达到目的更加妥当。

之所以这样做，一方面是因为 Python 的串是 immutable ，另一方面是因为 Python 的标准库具备比C标准库强得多“功能”。这是语言特性导致思维方法的变化。

当然，一个 C 程序员，看了一会儿 Python 手册，学到了Python语法，但没学到使用 Python 的最佳实践，也能写 C 风格的 Python 程序，可以用 C 的方式去操作 Python 的比特数组。这样的行为虽然在用 Python，但是不符合 Python 的编程范式，相当于仍然在写 C 程序，只不过披着用 Python 的语法的外衣。

另一个被广泛使用例子是[筛法求素数](http://en.wikipedia.org/wiki/Sieve_of_Eratosthenes)，相信很多人都写过。

在 golang 的文档中有提到一个[相当漂亮的实现](https://gist.github.com/3359265)。阅读过[SICP 第三话](http://mitpress.mit.edu/sicp/full-text/book/book-Z-H-24.html#%_sec_3.5.2)肯定会有似曾相识的感觉。这个实现与别的实现不同，它基于流而不是基于随时间变化的状态模型。这在函数式语言中是家常便饭，但是得益于 go 的 goroutine 和 channel，我们可以随心所欲地以这样干净的结构编写程序（当然 Python yield 也可以，不过go的实现中使用并发是那样自然）。

---

看上去我们的思维那么容易被语言这种外界因素左右，好像闻到了一种不可靠的味道。但是这种适应性让我们能够转换看待问题的角度，在解决问题时显示出它的价值。

有两大类有限状态自动机(FSA)被运用在串匹配领域：NFA 和 DFA。前者规模小，但是由于转换边不唯一，它的匹配速度远远落后于规模巨大但是转换边确定的后者。这样的结果是因为我们日常使用的通用架构更加适合于 DFA 的匹配算法。难道认为 NFA 就毫无意义么？不是的。一旦引入到 [FPGA](http://en.wikipedia.org/wiki/Field-programmable_gate_array) 硬件架构，让每次转换都能够并发进行，以 NFA 为基础的算法就能够凭借更小的规模更快得到解。

Alan Perlis 说：“对于一门新语言呢，如果没有影响到哥编程的思维方法，就不值得学它”。倒是一个很好的关于是否应该学习 X 语言的答案。
