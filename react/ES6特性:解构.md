# ES6特性:解构

在ES5里面，从某个object或者array读取值的时候需要

```javascript
var name = user.name;
var gender = user.gender;
```

ES6里面提供了解构，可以一行里读取多个属性或者值
```javascript
const {name, gender} = user;

arr = ['ann','jeny','bob'];

const [user1, user2, user3] = arr;
```