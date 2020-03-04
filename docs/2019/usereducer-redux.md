### 使用useContext和useReducer实现redux功能

#### 简介
&emsp;在接触React技术栈时，不可避免的要遇到Redux。作为一个较难理解的概念，相信我们大多数人都见到过下面几句话：

> - 如果你不知道是否需要 Redux，那就是不需要它。
> - 只有遇到 React 实在解决不了的问题，你才需要 Redux 。
> - Redux 和 React 没有关系，Redux 可以用在任何框架中。

&emsp;那么问题来了，究竟Redux是个什么东西，我们什么时间该用它呢？虽然很多解释都比较晦涩难懂，但是实际使用Redux的场景却很简单：不同组件共享数据状态。这个功能很简单，目的也很明确，我们可以使用React Hooks自带的useContext和useReducer来实现整个功能，从而帮助理解Redux。

#### useContext
&emsp;