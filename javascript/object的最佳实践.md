# object的最佳实践


在代码结束后，即使两个实例使用了同一个构造函数，它们也不再共享一个隐藏类。
动态删除属性与动态添加属性导致的后果一样。
最佳实践是把不想要的属性设置为 null。这样可以保持隐藏类不变 和继续共享，同时也能达到删除引用值供垃圾回收程序回收的效果。