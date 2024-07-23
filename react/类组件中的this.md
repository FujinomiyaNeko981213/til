# 类组件中的this

类中的方法不能直接使用this，有三种办法来让成员函数能访问到同一个this
1. 在构造函数中定义函数(不推荐，会让构造函数混乱)
```javascript
class ExplainBindingsComponent extends Component {
  constructor() {
    super();

    this.onClickMe = () => {
      console.log(this);
    }
  }

  render() {
    return (
      <button
        onClick={this.onClickMe}
        type="button"
      >
        Click Me
      </button>
    );
  }
}
```
2. 在构造函数中绑定this
```javascript
class ExplainBindingsComponent extends Component {
  constructor() {
    super();

    this.onClickMe = this.onClickMe.bind(this);
  }

   onClickMe(){
    console.log(this);
}

  render() {
    return (
      <button
        onClick={this.onClickMe}
        type="button"
      >
        Click Me
      </button>
    );
  }
}
```

3. 类方法可以通过 ES6 的箭头函数做到自动地绑定
```javascript
class ExplainBindingsComponent extends Component {
   onClickMe = () => {
    console.log(this);
  }
  render() {
    return (
      <button
        onClick={this.onClickMe}
        type="button"
      >
        Click Me
      </button>
    );
  }
}