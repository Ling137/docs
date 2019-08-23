# 测试

### 什么是测试

> 描述一种用来促进鉴定软件的正确性、完整性、安全性和质量的过程。换句话说，软件测试是一种实际输出与预期输出之间的审核或者比较过程。软件测试的经典定义是：在规定的条件下对程序进行操作，以发现程序错误，衡量软件质量，并对其是否能满足设计要求进行评估的过程。

### 目的

> 让开发者明确知道代码结果

### 常见的测试类型

-   单元测试 :从字面意思理解,写一段代码来测试一个单元 他有可能是一个 function，一个 module 一个 package 一个类
-   集成测试 :在单元测试的基础上，将所有模块按照设计要求（如根据结构图）组装成为子系统或系统，进行集成测试
-   样式测试 :UI 的样式测试为了测试我们的样式是否复合设计稿预期。同时通过样式测试我们可以感受当我们 code 变化带来的 ui 变化，以及他是否符合预期

### 测试分为（TDD & BDD）

> TDD：测试驱动开发（Test-Driven Development）测试驱动开发是敏捷开发中的一项核心实践和技术，也是一种设计方法论。 先编写单元测试用例代码， 测试代码确定需要编写什么产品代码。TDD 的基本思路就是通过测试来推动整个开发的进行，但测试驱动开发并不只是单纯的测试工作，而是把需求分析，设计，质量控制量化的过程。TDD 首先考虑使用需求（对象、功能、过程、接口等），主要是编写测试用例框架对功能的过程和接口进行设计，而测试框架可以持续进行验证。关注所有的功能是否被实现(每一个功能都必须有测试用例)

#### TDD 方法的特点：

> -   有利于更加专注软件设计；
> -   清晰地了解软件的需求；
> -   很好的诠释了代码即文档。
> -   TDD 更偏重与测试代码的功能是否实现正确，

### BDD：行为驱动开发（Behavior Driven Development）行为驱动开发是一种敏捷软件开发的技术，它鼓励软件项目中的开发者、QA 和非技术人员或商业参与者之间的协作,

主要是从用户的需求出发，强调系统行为。BDD 最初是由 Dan North 在 2003 年命名，它包括验收测试和客户测试驱动等的极限编程的实践，作为对测试驱动开发的回应

#### BDD 特点：

> -   关注整体行为是否符合整体预期，编写的每一段代码都有目的提供一个全面的测试用例集
> -   单元测试的目的是为了保证开发质量,减小测试成本,而手段是通过检查实际情况是否满足期望

#### 常见的测试 组合

1.  单元测试 (Mocha+chai) kaima+mocha,jest
2.  e2e 测试 selenium webdirver ,nightwatch,rize,
3.  API 测试 mocha+chai (supertest) ,rize,
4.  UI 还原性测试 backstop.js 、uirecorder、nightwatchjs
5.  性能测试 jemter

### 覆盖率

Istanbul 是 JavaScript 程序的代码覆盖率工具，以土耳其最大城市伊斯坦布尔命名。Istanbul 会对代码进行转换，生成语法树，然后在相应位置注入统计代码，执行之后根据注入的全局变量的值，统计代码执行的次数；在对代码的转换完成之后，Istanbul 会调用 test runner，例如 mocha，执行转换之后的代码的测试，生成测试报告。

链接地址:[ https://github.com/Silence520/QATest](https://github.com/Silence520/QATest)