# FE-knowledge-webpack 🏠
> webpack知识总结

#### 入口（entry）
  * 多入口：对象写法
```
const config = {
  entry: {
    app: './src/app.js',
    vendors: './src/vendors.js'
  }
 }
  ```
  * 单一入口：
```
const config = {
  entry: './path/to/my/entry/file.js'
};
```
对比：多入口写法可扩展性强，即可重用，可和其他配置组合使用（webpack-merge合并），更为推荐。
#### 出口（output）
#### loader
#### 插件（plugin）
#### 模式（mode）
#### 模块（modules）
#### reslove
#### 其他

