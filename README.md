# ReactLearn
# Hooks

## useState

## useEffect
- 副作用概念：
    - 纯函数：一个确切的参数在函数中运行后，一定能得到一个确切的值
    - 如果函数存在副作用，就不是一个纯函数，所谓副作用，指的是函数的结果不可控，不可预期
    - 常见的副作用有发送网络请求、添加一些监听的注册和取消注册，手动修改DOM，以前将这些副作用写作生命周期钩子函数中，现在书写在useEffect这个hook中
- 副作用的依赖
    - 副作用函数每次重新渲染后，都会重新执行，有时候需要设置依赖项，传递第二个参数，第二个参数为一个依赖数组
    - 如果想要副作用函数只执行一次，可以设置空数组作为依赖项，请求时要这样设置