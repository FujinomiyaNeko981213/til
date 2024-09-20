# for-in和for-of的区别

老记不住，写出来自己写一遍
for-in是遍历对象的属性名
for-in 语句是一种严格的迭代语句，用于枚举对象中的'''非符号'''键属性
```javascript
for(const propname in window){
    console.log(propname);
}
```

for-of是遍历可迭代对象，调用的是对方的next函数
for-of 语句是一种严格的迭代语句，用于遍历可迭代对象的元素

```javascript
for(const i of [2,4,6,8]){
    console.log(i);
}
```
![Uploading image.png…]()
