ES6工具链
要让Angular2应用跑起来不是件轻松的事，因为它用了太多还不被当前主流浏览器支持 的技术。所以，我们需要一个工具链：

toolchain

Angular2是面向未来的科技，要求浏览器支持ES6+，我们现在要尝试的话，需要加一些 垫片来抹平当前浏览器与ES6的差异：

systemjs - 通用模块加载器，支持AMD、CommonJS、ES6等各种格式的JS模块加载
es6-module-loader - ES6模块加载器，systemjs会自动加载这个模块
traceur - ES6转码器，将ES6代码转换为当前浏览器支持的ES5代码。systemjs会自动加载 这个模块。