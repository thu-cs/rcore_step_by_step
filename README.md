# 从零开始写 OS

## 前言

本系列文章记录了使用 Rust 编程语言编写一个小型操作系统的详细过程。每篇文章包含所需所有所需代码和相关知识点讲解。

- [GitHub（代码）](https://github.com/LearningOS/rcore_step_by_step)

- [GitBook（文档）](https://xy-plus.gitbook.io/rcore-step-by-step)

- [知乎专栏](https://zhuanlan.zhihu.com/c_1086573713289347072)

## 如何使用

为了方便起见，建议使用 [docker](http://www.runoob.com/docker/docker-tutorial.html) ，可以省去配置环境的功夫。

在工作目录下创建 **Makefile** ：

```Makefile
docker:
	sudo docker run -it --mount type=bind,source=$(shell pwd)/..,destination=/mnt panqinglin/rust_riscv bash
```

进入 docker 后，执行 `cd mnt` ，即可看见工作目录，然后就可以开始写代码啦！

> 每一章对应的源代码可以在 [GitHub](https://github.com/LearningOS/rcore_step_by_step) 的 commit 中找到， commit 号于每一篇文章的开头给出
