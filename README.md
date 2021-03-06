# 设计模式
仓库内容总结[图说设计模式](http://design-patterns.readthedocs.io/zh_CN/latest/index.html)和[刘伟设计模式](https://blog.csdn.net/lovelion/article/details/17517213)而来。

## 模式类型
- [创建型模式(Creational Pattern)](creational_pattern/creational-pattern.md)
    - 类创建型
        - Factory Method
    - 对象创建型
        - Abstract Factory
        - Builder
        - Prototype
        - Singleton
- [结构型模式(Structural Pattern)](structural_pattern/structural-pattern.md)
    - 类结构型模式
        - Adapter(类)
    - 对象结构型模式
        - Adapter(对象)
        - Bridge
        - Composite
        - Decorator
        - Facade
        - Flyweight
        - Proxy
- [行为型模式(Behavioral Pattern)](behavioural_pattern/behavioural-pattern.md)
    - 类行为型模式
        - Interpreter(解释器)
        - Template Method(模板方法)
    - 对象行为型模式
        - Chain of Responsibility(职责链)
        - Command(命令)
        - Iterator(迭代器)
        - Mediator(中介者)
        - Memento(备忘录)
        - Observer(观察者)
        - State(状态)
        - Strategy(策略)
        - Visitor(访问者)

## 模式理解
- 创建型模式关注对象的创建
- 结构型模式关注类或对象之间的组织关系
- 行为型模式关注类或对象间的交互和职责分配(就是用来干什么)

模式从本质上都是简化和分解类或对象，使易于扩展或封装性更好；一些相似的模式的区别最好从目的入手进行区分。

## 模式的目的准则
模式依据其目的可分为创建型、结构型、行为型。创建型模式与**对象的创建有关**，结构型模式**处理类或对象的组合**，行为型模式**对类或对象怎样交互和怎么分配职责进行描述**。

## 模式范围准则
指定模式主要是用于类还是用于对象。**类模式处理类和子类之间的关系，这些关系通过继承建立，是静态的，在编译时刻便确定下来了**。**对象模式处理对象间的关系，这些关系在运行时是可以变化的，更具动态性**。从某种意义上来说，几乎所有模式都使用继承机制，所以“类模式”只指那些**集中于处理类间关系的模式**，大部分模式都属于对象模式范畴。

创建型类模式将对象的部分创建工作延迟到子类，而创建型对象模式则将它延迟到另一个对象中。结构型类模式使用继承机制来组合类，而结构型对象模式则描述了对象的组装方式。行为型类模式使用继承**描述算法和控制流**，而行为型对象模式则描述了一组对象怎样协作完成单个对象所无法完成的任务。


## 设计模式原则
- 单一职责原则
    - 单个类应该有单一的职责，即一个类只做一件事情或者换一种说法就是一个类只能应对一种变化
- 开闭原则 ：目标
    - 对修改闭合对扩展开放
- 里氏替换原则 ：指导
    - 基类引用的地方可以透明的替换成子类对象，多态实现的基础
- 依赖倒置原则 ：手段
    - 抽象不应该依赖实现细节，反之细节应该依赖抽象；面向接口编程而非面向实现编程
- 接口隔离原则
    - 一个冗余的大接口，每次实现的时候都需要实现完全部方法，而部分方法又不需要用到；根据接口的功能进行拆分，大接口替换成小接口
- 迪米特法则
    - 一个软件实体不应该过多地与其他实体发生相互作用，又叫做只与你的直接朋友通信