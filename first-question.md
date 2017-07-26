今天不更新后台开发相关的课程，给大家安利一些学习资源。一个是Kubernetes相关的，一个是Golang相关的。

# Kubernetes

现在到处都在说微服务，微服务的经典玩法就是Kubernetes + Docker。我们组最近也在实践把服务切到Kubernetes上去，有几个好处：

1. 我们目前的服务部署是Docker + Ansible，自动化程度已经不错了。但是用Kubernetes的话，只用写好manifest配置，其他都万事大吉了，滚动升级也很方便。
2. 可伸缩性：可以自己设定规则来自动水平扩展。可以依据CPU使用量来伸缩，也可以自定义根据Latency来伸缩。
3. 简化代码：代替Zookeeper和ELB/EIP等服务发现机制，代替Zookeeper的leader election功能。
4. 资源调度：定义好Pod的Resource Request/Limit，具体部署到哪个节点也不用操心

要安利的是《Kubernetes指南》[http://feisky.xyz/kubernetes/](http://feisky.xyz/kubernetes/)，Feisky现就职于容器领域知名厂商[https://hyper.sh](https://hyper.sh)，也是Kubernetes的核心模块开发者。这份指南，对我来说看得比官方文档还舒服。

# Golang培训材料

Golang知名博主William Kennedy，也就是[GoingGo.net](https://www.goinggo.net)的创始人，现致力于Golang培训。有幸在GopherCon Singapore 2017现场听了Willian的演讲。他当时讲的是memory profiling相关的主题，深入浅出，也特别有激情。

他们一次培训是3天，一个班收3万美金，不超过15个学员。号称通过培训，你可以加速你的Golang经验6-12个月。2017年截至现在，已经举办了35场培训了。真是非常有意义的事情，又能得到可观的收入。

要安利的是培训材料开源了：[https://github.com/ardanlabs/gotraining](https://github.com/ardanlabs/gotraining)，感兴趣的朋友可自行学习。