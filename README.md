# angular2-webpack-systemJS
***
> Webpack是一个广受欢迎的模块打包器， 这个工具用来把程序源码打包到一些方便易用的块中，以便把这些代码从服务器加载到浏览器中，它是我们在文档中到处使用的SystemJS的一个优秀替代品

## webpack.common.js解读

* Webpack是基于NodeJS的一个工具，它能够从一个commonjs规范的JavaScript模块文件里读取配置。
这个配置文件是通过require语句导入依赖，然后将多个对象作为module.exports对象的属性导出。  

	    entries - 包体的入口文件。
	    resolve - 省略扩展名时如何解释文件名。
	    module.rules - module是一个对象，里面的rules属性用来决定文件如何加载。
	    plugins - 创建插件的实例。

* entry对象定义了三个包：

	    polyfills - 使得Angular应用能够运行在大多数的现代浏览器。
	    vendor - 第三方依赖，如Angular、lodash和bootstrap.css。
	    app - 应用代码。

## Commands

###### install dependencies
	npm install

###### start dev server
	npm start

###### create build for production
	npm run build

参考自 **ANGULAR** 之 [Webpack 简介](https://angular.cn/docs/ts/latest/guide/webpack.html "使用基于 Webpack 的工具创建 Angular 应用")
