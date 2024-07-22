# npm包管理

最基础的应用，新建一个文件夹然后在文件夹内初始化

```bash
npm init -y

```
如果省略初始化程序（仅通过调用 npm init ），init 将回退到旧的 init 行为。它会问你一堆问题，然后为你写一个package.json。它将尝试根据现有字段、依赖项和所选选项做出合理猜测。它是严格附加的，因此它将保留已设置的所有字段和值。您还可以使用 -y / --yes 完全跳过调查问卷。

全局安装某个包
```bash
npm install react -g

```

在当前安装某个包
```bash
npm install react

```

卸载某个包
```bash
npm uninstall react

```