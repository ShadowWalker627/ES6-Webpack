# ES6-Webpack
ES6+Webpack开发配置
####遇到的问题：
* 1.--port 8081  修改默认端口
* 2.babel-preset-stage-3：此插件用于ES7草案涉及的内容，一开始没有配这个，导致扩展运算符‘...’不能被解析，需要在loader中添加：
        ```
          query: {
              presets: ['es2015', 'stage-3']
          }
        ```
