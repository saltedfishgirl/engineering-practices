# Code Review开发人员指南


## 简介{#intro}
代码审查是一个除了一段代码的作者之外还有其他人检查该代码的过程。

在Google，我们使用代码审查来维护代码和产品的质量。

此文档是Google代码审核流程和政策的规范说明。

此页概述了我们的代码审阅过程。本指南还有另外两个大型文档：

- **[如何进行代码审查](reviewer/)**：代码审查员的详细指南。
- **[CL作者指南](developer/)**：正在进行审核的CL的开发人员详细指南。


## 代码审查员在寻找什么？{#look_for}
代码审查应该考虑：

- 设计：代码是否设计良好，适合你的系统？
- 功能：代码的行为是否符合作者的预期？代码的行为方式对用户有好处吗？
- 复杂性：代码是否可以变得更简单？将来遇到这种代码时，另一个开发人员是否能够轻松地理解和使用它？
- 测试：代码是否有正确且设计良好的自动化测试？
- 命名：开发人员是否为变量、类、方法等选择了清晰的名称？
- 点评：点评是否清晰有用？
- 样式：代码是否遵循我们的[样式指南](http://google.github.io/styleguide/)？
- 文档：开发人员是否也更新了相关文档？
有关详细信息，请参见 **[如何进行代码审查](reviewer/)**。

### 挑选最佳评审者{#best_reviewers}
一般来说，你希望找到能够在合理的时间内回复你的审查的 **最佳** 评审者。

最好的评审者是能够对您正在编写的代码进行最彻底、最正确的评审的人。这通常意味着代码的评审者，可能是文件所有者中的人，也可能不是。有时，这意味着要求不同的人来审查CL的不同部分。
如果您找到了理想的评审者，但他们不空闲时，你至少应该在更改时抄送他们。

### 当面评审{#in_person}
如果您与有良好代码审查资质的人结对编程一段代码，那么该代码将被视为已审核。

还可以进行面对面的代码审查，当变更的开发人员与评审者交谈时，评审者提出了问题。

### 另见{#seealso}
- [如何进行代码审查](reviewer/)：代码审查员的详细指南。
- [CL作者指南](developer/)：正在进行审核的CL的开发人员详细指南.
