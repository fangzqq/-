# xpath 与 lxml

## xpath 基本用法

XPath 是一门在 XML 文档中查找信息的语言。XPath 可用来在 XML 文档中对元素和属性进行遍历。

XML 中的节点关系包括：

- parent, 父
- children, 子
- sibling, 同胞
- ancestor, 先辈
- descendant, 后代

### 节点选取

XPath 使用路径表达式在 XML 文档中选取节点。节点是通过沿着路径或者 step 来选取的：

- `nodename`, 选取此节点的所有子节点
- `/`, 从根节点选取
- `//`, 从匹配选择的当前节点选择文档中的节点，而不考虑它们的位置
- `.`, 选取当前节点
- `..`, 选取当前节点的父节点
- `@`, 选取属性


### 谓语（Predicates）

谓语用来查找某个特定的节点或者包含某个指定的值的节点。谓语被嵌在方括号中。

### 选取未知节点

XPath 通配符可用来选取未知的 XML 元素：

- `*`, 匹配任何元素节点
- `@*`, 匹配任何属性节点
- `node()`, 匹配任何类型的节点


参考自知乎：https://zhuanlan.zhihu.com/p/29436838
