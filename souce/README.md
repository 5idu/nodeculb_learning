Nodeclub
=

[![build status][travis-image]][travis-url]
[![codecov.io][codecov-image]][codecov-url]
[![David deps][david-image]][david-url]
[![node version][node-image]][node-url]

[travis-image]: https://img.shields.io/travis/cnodejs/nodeclub/master.svg?style=flat-square
[travis-url]: https://travis-ci.org/cnodejs/nodeclub
[codecov-image]: https://img.shields.io/codecov/c/github/cnodejs/nodeclub/master.svg?style=flat-square
[codecov-url]: https://codecov.io/github/cnodejs/nodeclub?branch=master
[david-image]: https://img.shields.io/david/cnodejs/nodeclub.svg?style=flat-square
[david-url]: https://david-dm.org/cnodejs/nodeclub
[node-image]: https://img.shields.io/badge/node.js-%3E=_4.2-green.svg?style=flat-square
[node-url]: http://nodejs.org/download/

## 介绍

Nodeclub 是使用 **Node.js** 和 **MongoDB** 开发的社区系统，界面优雅，功能丰富，小巧迅速，
已在Node.js 中文技术社区 [CNode(http://cnodejs.org)](http://cnodejs.org) 得到应用，但你完全可以用它搭建自己的社区。

## 安装部署

*不保证 Windows 系统的兼容性*

线上跑的是 [Node.js](https://nodejs.org) v4.4.0，[MongoDB](https://www.mongodb.org) 是 v3.0.5，[Redis](http://redis.io) 是 v3.0.3。

```
1. 安装 `Node.js/io.js[必须]` `MongoDB[必须]` `Redis[必须]`
2. 启动 MongoDB 和 Redis
3. `$ make install` 安装 Nodeclub 的依赖包
4. `cp config.default.js config.js` 请根据需要修改配置文件
5. `$ make test` 确保各项服务都正常
6. `$ node app.js`
7. visit `http://localhost:3000`
8. done!
```

## 测试

跑测试

```bash
$ make test
```

跑覆盖率测试

```bash
$ make test-cov
```

## 贡献

有任何意见或建议都欢迎提 issue，或者直接提给 [@alsotang](https://github.com/alsotang)

## License

MIT

## package.json中依赖注释

```
    "async":为了解决嵌套金字塔,和异步流程控制而生
    "bcryptjs":加密模块
    "body-parser": 用于解析客户端请求的body中的内容
    "bytes": 将字符串转为字节，反之亦然
    "colors": 使用不同的颜色和风格在控制台渲染输出文字
    "compression": 压缩中间件（支持deflate、gzip）
    "connect-busboy": 解析传入的HTML表单数据
    "connect-redis": redis session存储中间件
    "cookie-parser": 使用签名来解析客户端cookie的中间件
    "cors": 跨域请求中间件
    "csurf": 用来防止CSRF(跨站请求伪造)攻击
    "data2xml": 将数据转为XML格式
    "ejs-mate": ejs模板引擎，支持partial功能
    "eventproxy": 使用事件式编程的思维来解决深度callback嵌套问题
    "express": NodeJS web框架
    "express-session": express web框架session中间件
    "helmet": 增加express应用的安全中间件
    "ioredis": redis使用中间件
    "jpush-sdk": 提供 JPush 服务端接口的 Node 封装，与 JPush Rest API 组件通信
    "loader-builder": 将源码翻译为原生的JavaScript和CSS,压缩JavaScript和CSS文件，减少文件体积,合并多个文件，减少请求数量,计算文件签名，利于增量式发布
    "loader": Node静态资源加载器,线上、线下对静态资源进行合并和压缩 
    "lodash": lodash工具库
    "log4js": 记录log日志
    "markdown-it": Markdown 解析器
    "memory-cache": 内存缓存
    "method-override": 容许一些不支持PUT、DELETE 等方法的客户端浏览器使用这些方法
    "moment": 日期解析、验证操作、格式化日期
    "mongoose": 操作MongoDB CRUD
    "multiline": 解决多行字符串拼接繁琐出错问题
    "node-uuid": 已被uuid替代，uid随机生成器
    "nodemailer": e-mail sending
    "nodemailer-smtp-transport": smtp e-mail sending
    "oneapm": 实时监控运行程序，抓取缓慢的程序代码和SQL语句
    "passport": 身份认证中间件
    "passport-github": github身份认证中间件
    "pm2": 自动启动程序
    "qn": 七牛云存储
    "ready": events处理
    "request": HTTP request client
    "response-time": 记录响应时间
    "superagent": 客户端请求代理模块
    "utility": 有用的工具集合模块
    "validator": 字符串验证
    "xmlbuilder": xml生成器
    "xss": 防止xss攻击
    "errorhandler": error处理模块
    "istanbul": 代码覆盖率测试模块
    "loader-connect": 静态资源编译器
    "mm": 模拟fs、http访问等
    "mocha": 测试框架
    "nock": module test
    "pedding": 单元测试工具
    "should": 断言测试工具
    "supertest": http test 工具
```