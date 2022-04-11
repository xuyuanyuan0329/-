

#### The concept of software testing. Basic definitions. 软件测试的概念。 基本定义。

Software testing is the process of evaluating and verifying that a software product or application does what it is supposed to do. The benefits of testing include preventing bugs, reducing development costs and improving performance. 软件测试是评估和验证软件产品或应用程序是否完成了它应该做的事情的过程。测试的好处包括防止错误、降低开发成本和提高性能。

#### Testing goals. Classification of tests. 测试目标。 测试分类。

– Defect detection – 缺陷检测
– Increasing confidence in the level of quality – 提高对质量水平的信心
– Providing information for decision making – 为决策提供信息
– Defect prevention – 缺陷预防

Classification:

There are two dimensions: *test level* and *test type* 测试有两个维度

###### Test level:

Unit test, Integration Test, System test, Acceptance Test. 单元测试、集成测试、系统测试、验收测试。

###### Test type:

Functional Testing, Nonfunctional Testing, Performance Testing, Security Testing, Regression Testing 功能测试、非功能测试、性能测试、安全测试、回归测试

[More details](https://www.informit.com/articles/article.aspx?p=2730111&seqNum=3) (按住ctrl点击可直接打开)

#### Unit testing. The concept of a unit. 单元测试。 模块的概念。

*Unit testing* is writing quick, low-level tests for a small part of a system. Unit can be a method, a function, a class or a program unit. Usually unit is the simplest and single one.

#### V-shaped model. *Static* and *dynamic testing*. V 形模型。 静态和动态测试。

![image-20220310141938749](C:\Users\TheHs\AppData\Roaming\Typora\typora-user-images\image-20220310141938749.png)

*Static testing* is about the prevention of defects but *Dynamic testing* is about finding and fixing the defects. *Static testing* does the verification process while *Dynamic testing* does the validation process. *Static testing* is performed before compilation whereas *Dynamic testing* is performed after compilation.

静态测试是关于预防缺陷，而动态测试是关于发现和修复缺陷。静态测试执行验证过程，而动态测试执行验证过程。静态测试在编译之前执行，而动态测试在编译之后执行。

静态测试不包含代码执行，可以手动测试或者自动测试。通常是非正式的端到端控制、检查。

动态测试是启动模块、模块组、整个系统。

#### Validation and verification. Black and white box testing. 验证和验证。 黑白盒测试。

**Validation** is about Expectations check. Does the software meet user requirements? If we want to make a pie, validation is check if the pie is full of *meat or vegetarian or sweet*? Have we done the right thing?

**验证**是关于期望检查。软件是否满足用户要求？如果我们想做派，验证是检查派是肉派，素派还是甜口派？做的对吗？符不符合要求的方向？

**Verification** is about Internal quality management. Does the software fulfill the requirements of the specification? How is its *size, doneness, filling and something* else? Have we done the thing right?

**验证**是关于内部质量管理。软件是否满足规范的要求？它的*大小、熟度、内陷和其他的参数*如何？做的好不好，做的质量怎么样？

##### Black and white box testing

Black box testing is considered high-level testing, which means that its main goal is to test functionalities from the behavioral point of view. White box testing, also known as clear box testing, happens when you have insight into the code and/or general knowledge about the architecture of the software in question.

黑盒测试被认为是高级测试，这意味着它的主要目标是从行为的角度测试功能。当您深入了解代码和/或有关软件架构的一般知识(细节)时，就会发生白盒测试，也称为明盒测试。



**黑盒测试**一直产品的功能设计规格，可以进行测试证明每个实现了的功能是否符合要求。
**白盒测试：**一直产品的内部工作过程，可以通过测试证明每种内部操作都符合设计规格要求，所有内部成分是否进行检查

[More details in Chinese.](https://blog.csdn.net/lemo_ice/article/details/102474858)

#### Test case, test scenario and test coverage. 测试用例、测试场景和测试覆盖率。

For a **test case**, we should input some data or do some control operations. And set the preconditions, execution conditions and postconditions. Set the expected result before the test. Then program will compare the actual result and expected result and output the result.

对于一个测试用例，我们应该输入一些数据或者做一些控制操作。并设置前置条件、执行条件和后置条件。在测试之前设置预期的结果。然后程序将比较实际结果和预期结果并输出结果。

**Scenario testing** is a type of *testing* carried out using *scenarios* derived from the use cases.

We can read the documentation for the project and know design user will do and then design the test case.

**场景测试**是一种使用源自用例的*场景* 进行的*测试*。

我们可以阅读项目的文档并知道设计用户会做什么，然后设计测试用例。

**Test coverage** is defined as a metric in Software Testing that measures the amount of testing performed by a set of test. We need to know how to test it? How much memory will it take? How long it will be executed on a specific CPU? 

#### Equivalence analysis. 等价分析。

**Equivalence tests** are a variation of hypothesis tests used to draw statistical inferences from observed data. The good example is about bank. If there are lots of customers and they want to save the money. And there are some limit about the amount. We can just test some limit values. Like 0, -1, 100, 1000. We can replace most values by testing some special values. This is *Equivalence tests*.

#### Decision tables and transition tables. 决策表和转换表。

**Decision table:**

● Used in systems with complex logic, description of the state machine
● Can include a large set of conditions (usually true-false), and actions

**决策表：**

● 用于逻辑复杂的系统，状态机的描述
● 可以包含大量条件（通常为真-假）和操作

**Transition table**:

It allows you to select states and their combinations that can be omitted. Cover certain lines with tests

**转换表**：

它允许您选择可以省略的状态及其组合。 用测试覆盖某些行

#### Regression testing. 回归测试。

**Regression testing** (rarely, non-regression testing) is re-running functional and non-functional tests to ensure that previously developed and tested software still performs after a change.

**回归测试**（很少是非回归测试）是重新运行功能和非功能测试，以确保先前开发和测试的软件在更改后仍然可以执行。

#### JUnit library. API features. The junit.framework.Assert class. JUnit 库。 API 功能。 junit.framework.Assert 类。

**Junit** is a classical library for JAVA Testing. It has some annotations like @Test can tell the program we want to use unit test for this function or method. @BeforeEach and @BeforeAll can let us configure before the test. And one of the most important parts is the **assertion class**. There are some funtions like assertEquals, assertSame, assertTrue, assertThrows, assertTimeout… We can use them to compare the actual result and the expected result. We can check if the program throws the correct exceptions and some else.

**Junit** 是一个经典的 JAVA 测试库。 它有一些注解，比如@Test 可以告诉程序我们要对这个函数或方法使用单元测试。 @BeforeEach 和@BeforeAll 可以让我们在测试前进行配置。 最重要的部分之一是**断言类**。 有一些函数，如assertEquals、assertSame、assertTrue、assertThrows、assertTimeout……我们可以用它们来比较实际结果和预期结果。 我们可以检查程序是否抛出了正确的异常和其他一些异常。

#### Differences between JUnit 3 and JUnit 4. JUnit 3 和 JUnit 4 之间的差异。

JUnit 4 is based on the Java 5. We can use the annotation to build the test class and method. 

It also has generics and static import features.

JUnit3 need to extends TestCase class then we write the test methods.

JUnit3 we need to name the function like “testFuction1”, “testFunction2”. The name must start with “test”.

In JUnit4, there is no limit about naming.

JUnit 4 基于 Java 5。我们可以使用注解来构建测试类和方法。

它还具有泛型和静态导入功能。

JUnit3需要扩展TestCase类，然后我们编写测试方法。

JUnit3 我们需要将函数命名为“testFuction1”、“testFunction2”。 名称必须以“test”开头。

在 JUnit4 中，命名没有限制。



**PS:** Differences between JUnit4 and JUnit5. 

One test runner can only execute tests in JUnit 4 at a time (e.g. SpringJUnit4ClassRunner or Parameterized ). JUnit 5 allows multiple runners to work at the same time. JUnit5 can support JAVA8 and JUnit4 never advanced beyond JAVA7. So JUnit4 miss out some features from JAVA 8.

And in JUnit4 we usually use the annotation to set the expected exception.

```java
@Test(expected = Exception.class)
public void shouldRaiseAnException() throws Exception {
    // ...
}
```

Now we can use the method assertThrows:

```java
public void shouldRaiseAnException() throws Exception {
    Assertions.assertThrows(Exception.class, () -> {
        //...
    });
}
```

