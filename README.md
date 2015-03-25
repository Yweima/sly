# [Sly](http://darsa.in/sly)

Sly是一个基于项的导航的JavaScript库，支持的一个方向的滚动。

[demo1](http://www.lanrentuku.com/down/js/tupian-901/)

[demo2](http://darsa.in/sly/)


## 一、Sly简介

sly一种先进的单向滚动项目导航支持JavaScript库。
它可以用来作为一个简单的滚动条替换，作为一种先进的基于项目的导航工具，或作为一个伟大的导航和动画的网站界面的视差。这是一个强大的开发者友好的API，提供了一些非常有用的方法让你控制一切了。

+ 1、依赖
  jQuery 1.7 +
  就是这样。你不需要详细说明jQuery UIsly：）在未来的日子里，我想把jQuery的依赖，并转换到一个可重用的狡猾组件。
+ 2、兼容性
  在每个桌面浏览器sly作品，由于一些神圣的干预，甚至在IE6 +，但这是一个完整的事故。IES低于8没有正式支持：）。
+ 3、手机
  sly触摸事件，我通常试图使它工作无处不在，但事实是，移动不测试。如果你想帮助，欢迎你：）。

## 二、性能

性能为了实现最敏感的经验与流畅的动画可能有很多重点放在性能。
sly有一个自定义的高性能基于渲染动画动画时间接口直接为其需要写。这提供了一个优化的60帧的渲染，和设计还接受宽松的功能jQuery宽松的插件，所以你不会事件通知，sly动画不jQuery：）。
元素的动画是通过GPU加速的翻译转换，从而迅速提高渲染速度的浏览器支持它，而那些喜欢绝对定位的后备
帮助减少帧频率下降由于不可避免的JavaScript垃圾收集代码优化，降低垃圾产生一个合理的最低。
提供一个超级敏感的和光滑的同步时，拖动滚动条柄，sly使用基于目的的动画功能的而不是一个时间同步的因素控制的基础（渐变）的动画，使用这种类型的情况下是不合适的，并导致一个波涛汹涌，和未抛光的经验。另一个好处编写您自己的动画渲染：）。
这是较早的版本（使用之间的差异jquery.fn.animate与未优化的代码）和sly当前状态：
before_after

## 三、例子

[Horizontal](http://darsa.in/sly/examples/horizontal.html)

[Vertical](http://darsa.in/sly/examples/vertical.html)

[Full page](http://darsa.in/sly/examples/fullpage.html)

[Infinite scrolling](http://darsa.in/sly/examples/infinite.html)

[Parallax mode](http://darsa.in/sly/examples/parallax.html)


所有的例子（除视差之一）是使用一个调用通过jQuery的代理，因为有些人认为是只看例子认为jQuery是一种独立的语言也无法处理的原生JavaScript。这会帮助降低“帮助我使它的工作”的问题的报告。
更高级的用户可以阅读的文件，发现所有的电力和很酷的东西，新的sly()提供：）

## 四、文档

[Markup HTML & CSS](https://github.com/darsain/sly/wiki/Markup)

[Calling](https://github.com/darsain/sly/wiki/Calling)

[Options](https://github.com/darsain/sly/wiki/Options)

[Properties](https://github.com/darsain/sly/wiki/Properties)

[Methods](https://github.com/darsain/sly/wiki/Methods)

[Events](https://github.com/darsain/sly/wiki/Events)

[Parallax](https://github.com/darsain/sly/wiki/Parallax)


项目地址：http://darsa.in/sly/

下载地址：https://github.com/darsain/sly/raw/master/dist/sly.min.js

***

JavaScript library for one-directional scrolling with item based navigation support.

Sly supports navigation with:

- mouse wheel scrolling
- scrollbar (dragging the handle or clicking on scrollbar)
- pages bar
- various navigation buttons
- content dragging with mouse or touch
- automated cycling by items or pages
- lots of super useful methods

... and has a powerful & developer friendly API!

That's all build around a custom [highly optimized animation rendering](http://i.imgur.com/nszjJBZ.png) with
requestAnimationFrame, and GPU accelerated positioning with fallbacks for browsers that don't support it.

#### Dependencies

- jQuery 1.7+

#### Compatibility

Works everywhere, even in IE6+ abominations, but that is a complete accident :) IE 6-7 are not officially supported.

### [Forum](https://groups.google.com/d/forum/sly-js)

Forum is for questions. Issues are for bug reports and feature requests. Don't mix the two :)

## Usage

Constructor:

```js
var options = {
	horizontal: 1,
	itemNav: 'basic',
	speed: 300,
	mouseDragging: 1,
	touchDragging: 1
};
var frame = new Sly('#frame', options).init();
```

jQuery proxy:

```js
var options = {
	horizontal: 1,
	itemNav: 'basic',
	speed: 300,
	mouseDragging: 1,
	touchDragging: 1
};
$('#frame').sly(options);
```

jQuery proxy is good when you want to create an instance and forget about it. For anything more complex, like using methods, events, accessing instance properties, ... use the constructor and work with the instance directly.

## Download

Latest stable release:

- [Production `sly.min.js`](https://raw.github.com/darsain/sly/master/dist/sly.min.js) - 16KB, 7KB gzipped
- [Development `sly.js`](https://raw.github.com/darsain/sly/master/dist/sly.js) - 55KB

When isolating issues on jsfiddle, you can use this URL:

- [http://darsain.github.io/sly/js/sly.min.js](http://darsain.github.io/sly/js/sly.min.js)

## Documentation

Can be found in the [docs](https://github.com/darsain/sly/tree/master/docs) directory.

## Contributing

Please, read the [Contributing Guidelines](CONTRIBUTING.md) for this project.

