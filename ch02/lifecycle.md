### 生命周期方法

- componentWillUpdate()之前触发，给你有一个机会返回false以取消更新

  当你的组件再次渲染时，在render()方法前调用（在组件的props或state发生改变时会触发该方法）

- componentDidUpdate()

  在render()函数执行完毕，并且更新的组件已被同步到DOM后立即调用。该方法不会在初始化渲染时触发

- componentWillMount()

  在新节点出入DOM结构之前触发

- componentDidMount()

  在新节点插入DOM结构之后触发

- componentWillUnmount()

  在组件从DOM中移除时立刻触发

- shouldComponentUpdate(newProps, newState)

  这个方法在componentWillUpdate()之前触发，给你有一个机会返回false以取消更新，这意味着render()方法将不会被调用