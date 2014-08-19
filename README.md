# Zepto.js

原始项目见[Zepto](https://github.com/madrobby/zepto)

## 本分支提供的特性

1、兼容`SeaJS`模块，不需要自己改源码加 `define`头

2、支持`$.noop`、`$.now`、`$.error`，其用法同`jQuery`

3、添加`withCredentials`支持，修复在`xhr.open`前设置`withCredentials`报`INVALID_STATE_ERR`错误的问题

4、修复2个手指连续点击或滑动导致的`evaluating 'touch.el.trigger'`错误的问题

5、修复三星机型`touchmove`过于敏感导致`longTap`事件失效的问题

## 构建

`dist`目录里有已构建好的版本，可以直接使用，集成了`zepto callbacks deferred event ajax form touch`模块，如果需要自定义模块的话就需要手动构建了

1、安装[NodeJS](http://nodejs.org/)

2、clone本项目的源代码

3、进入源代码目录，运行下面的命令安装依赖包

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
