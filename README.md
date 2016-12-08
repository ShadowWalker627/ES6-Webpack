# ES6-Webpack
ES6+Webpack开发配置<br/>
  遇到的问题：<br/>
    1：--port 8081  修改默认端口<br/>
    2：babel-preset-stage-3：此插件用于ES7草案涉及的内容，一开始没有配这个，导致扩展运算符‘...’不能被解析，<br/>
        需要在loader中添加：<br/>
          query: {<br/>
              presets: ['es2015', 'stage-3']<br/>
          }<br/>
