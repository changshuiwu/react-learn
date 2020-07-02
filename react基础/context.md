### Consumer、ContextType、useContext的区别
* Consumer 组件在类组件和函数组件中都可以使用。作为消费组件，可以有多个Provider传值，接收多个全局变量。  
* ContextType 属性作为静态成员，在函数组件中无法使用。ContextType会被重新赋值为一个新的Context对象，Context只能使用一个Context，就算有多个传值，也只会接收一个值。
* useContext 是函数组件中的方法。 可以有多个Provider传值，接收多个全局变量，useContext解决了Consumer组件书写繁琐的问题，还解决了ContextType只能使用一个Context的问题。