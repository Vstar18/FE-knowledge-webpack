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

---------
#### 出口（output）
 属性告诉 webpack 在哪里输出它所创建的 bundles，以及如何命名这些文件
 
---------
#### loader   
 * 作用：用于模块的源代码进行转换成js（css，img等都可以处理成js，因为webpack只认识js文件）
 * 使用方式： 
 1. 内置配置，我们常用的webpack.config文件
 2. CLI，shell命令
    ```
    webpack --module-bind jade-loader --module-bind 'css=style-loader!css-loader'
    ```
 3. import语句显示的指明
      通过所有规则及使用 !
     ```
     import Styles from 'style-loader!css-loader?modules!./styles.css';
     ```
     > 推荐使用内置配置的方式   
     > >1.可以减少源码量   
     > > 2. 可以在发生问题的使用迅速定位
     
---------

#### 插件（plugin）
#### 模式（mode）
#### 模块（modules）
#### reslove
#### 其他

