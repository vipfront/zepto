# Zepto.js

原始项目见[Zepto](https://github.com/madrobby/zepto)

## 本分支提供的特性

1、添加`withCredentials`支持，修复在`xhr.open`前设置`withCredentials`报`INVALID_STATE_ERR`错误的问题

2、修复2个手指连续点击或滑动导致的trigger相应时间出错的问题

## 构建

1、安装[NodeJS](http://nodejs.org/)

2、clone本项目的源代码

3、进入源代码目录，安装依赖包

~~~ sh
$ npm install
~~~

4、运行脚本构建自己的Zepto吧

~~~ sh
$ npm run-script dist
~~~

5、修改make第42行可以定制自己需要的模块，或者如下操作

~~~ sh
$ MODULES="zepto event data" npm run-script dist
~~~

## 单元测试

~~~ sh
npm test
~~~