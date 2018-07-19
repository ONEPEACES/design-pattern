# 行为型模式
行为型模式是对在不同的对象之间划分责任和算法的抽象化。

行为型模式不仅仅关注类和对象的结构，而且重点关注它们之间的相互作用。

通过行为型模式，可以更加清晰地划分类与对象的职责，并研究系统在运行时实例对象之间的交互。在系统运行时，对象并不是孤立的，它们可以通过相互通信与协作完成某些复杂功能，一个对象在运行时也将影响到其他对象的运行。

行为型模式也分为类行为型模式和对象行为型模式：
- 类行为型模式：类的行为型模式使用继承在几个类之间分配行为（使用继承描述算法和控制流），类行为型模式主要通过多态等方式来分配父类与子类之间的职责
- 对象行为型模式：对象行为型模式使用对象的聚合关联关系来分配行为，对象行为型模式主要通过对象关联等方式来分配两个或多个类的职责。根据“合成复用原则”，系统应该尽量使用关联关系取代继承关系，因此大部分行为型模式都是对象行为型模式

## 包含模式
类行为模式：
- Template Method（模板方法）
- Interpreter（解释器）

对象行为型模式：
- Command（命令）
- Chain of Responsibility（职责链）
- Iterator（迭代器）
- Mediator（中介）
- Memento（备忘录）
- Observer（观察者）
- State（状态）
- Strategy（策略）
- Visitor（访问者）