# 紧急情况
有时，紧急CL必须尽快通过整个代码审查过程。


## 什么是紧急情况？{#what}

紧急CL将是一个小变化：允许主要发布继续而不是回滚，修复显着影响用户生产的错误，处理紧迫的法律问题，关闭主要安全漏洞等。

在紧急情况下，我们确实关心整个代码审查过程的速度，而不仅仅是[响应的速度]((reviewer/speed.md))。仅在这种情况下 ，审核人员应该更关心审核的速度和代码的正确性（它实际上是否解决了紧急情况？）。此外（也许显然）这些评论应该优先于所有其他代码评论，当它们出现时。

但是，在紧急情况得到解决后，您应该再次查看紧急CL并给予他们[更彻底的审查]((reviewer/looking-for.md))。


## 什么不是紧急情况？{#not}

需要说明的是，以下情况并非紧急情况：

- 想要在本周而不是下周推出（除非有一些实际的[硬期限](#deadlines)启动，例如合作伙伴协议）。
- 开发人员已经开发了很长时间的功能，他们真的想要获得CL。
- 审稿人都在另一个时区，目前正在夜间或他们离开现场。
- 这是星期五的一天结束，在开发者离开周末之前获得这个CL会很棒。
- 一位经理表示，由于[软（非硬）截止日期](#deadlines)，此审查必须完成并且今天检查CL 。
- 回滚导致测试失败或构建破坏的CL。
等等。

### 什么是硬截止日期？{#deadlines} 
一个硬期限是如果你错过它会发生灾难性的事情。例如：

- 在特定日期提交您的CL对于合同义务是必要的。
- 如果在某个日期之前没有发布，您的产品将在市场上完全失败。
- 一些硬件制造商每年只发送一次新硬件。如果您错过了向他们提交代码的截止日期，那么这可能是灾难性的，具体取决于您尝试发布的代码类型。

延迟发布一周并不是灾难性的。错过重要会议可能是灾难性的，但往往不是。

大多数截止日期都是软截止日期，而非最后期限。它们表示希望在特定时间内完成某项功能。它们很重要，但你不应该牺牲代码健康来制作它们。

如果您的发布周期很长（几周），那么在下一个周期之前就可能会牺牲代码审查质量来获取功能。然而，这种模式如果重复，是项目建立压倒性技术债务的常用方式。如果开发人员在周期结束时经常提交CL，只需要进行表面评审就必须“进入”，那么团队应该修改其流程，以便在周期的早期发生大的功能变化，并有足够的时间进行良好的审核。
