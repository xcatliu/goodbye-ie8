# Goodbye IE8

> As [more and more JavaScript frameworks and libraries dropped IE8 support](#timeline), It's time to say goodbye to IE8.

Let's work together to promote the evolution of the browser!

## What to Do

### 1. Add alert message for IE8 users

Copy this code as the first child element of `<body>`:

```html
<!--[if lt IE 9]>
  <p style="text-align: center!important; margin: 0 0 0.5em!important; background-color: #d9534f!important; color: #fff!important; padding: 0.5em 1em!important;">You are using an <strong>outdated</strong> browser. Please <a style="color: #fff!important" href="http://browsehappy.com/?locale=en">upgrade your browser</a> to improve your experience.</p>
<![endif]-->
```

Preview what alert message will show on IE 8 and lower: http://xcatliu.github.io/goodbye-ie8

Code was forked from https://github.com/h5bp/html5-boilerplate/blob/master/src/index.html

中文版：

```html
<!--[if lt IE 9]>
  <p style="text-align: center!important; margin: 0 0 0.5em!important; background-color: #d9534f!important; color: #fff!important; padding: 0.5em 1em!important;">您正在使用<strong>过时的</strong>浏览器，请<a style="color: #fff!important" href="http://browsehappy.com/">升级你的浏览器</a>获得更好的用户体验。</p>
<![endif]-->
```

### 2. Drop css hacks for IE8

[CSS Hacks][Browser Specific Hacks] used to be an effective way to keep browsers looks good, now let's drop them.

// TODO: Best Practice: try css preparsers like [sass](http://sass-lang.com/) or [less](http://lesscss.org/) with [postcss](https://github.com/postcss/postcss) plugins.

### 3. Feel free to use ES5 features

According to [Compatibility Table for ES5], IE9+ supports all ES5 features. It's safe to use them without [es5-shim](https://github.com/es-shims/es5-shim).

### 4. Remove HTML5 Shiv

The [HTML5 Shiv](https://github.com/aFarkas/html5shiv) enables use of HTML5 sectioning elements in IE8. It's not necessary now.

### 5. And else?

// TODO

## Timeline

- 2006-03-?? IE8 development started
- 2008-03-05 IE8 Beta 1 released
- 2009-03-19 IE8 released
- 2013-04-18 [jQuery 2.0 leaves behind the older Internet Explorer 6, 7, and 8 browsers]
- 2013-12-15 [AngularJS 1.3 discontinues support for Internet Explorer 8]
- 2014-04-08 [Support for Windows XP ended April 8th, 2014]
- 2015-08-19 [Bootstrap v4 dropped IE8 support]
- 2016-01-12 [Support for older versions of Internet Explorer ended on January 12th, 2016]
- 2016-01-12 [Discontinuing IE 8 Support in React DOM]

// TODO: Complete the timeline

## Contributing

Any issue or pull requests are welcomed.

## References

- [Browser Specific Hacks]
- [Compatibility Table for ES5]
- https://en.wikipedia.org/wiki/Internet_Explorer_8
- [jQuery 2.0 leaves behind the older Internet Explorer 6, 7, and 8 browsers]
- [AngularJS 1.3 discontinues support for Internet Explorer 8]
- [Support for Windows XP ended April 8th, 2014]
- [Bootstrap v4 dropped IE8 support]
- [Support for older versions of Internet Explorer ended on January 12th, 2016]
- [Discontinuing IE 8 Support in React DOM]

[Browser Specific Hacks]: https://css-tricks.com/snippets/css/browser-specific-hacks/
[Compatibility Table for ES5]: http://kangax.github.io/compat-table/es5/
[jQuery 2.0 leaves behind the older Internet Explorer 6, 7, and 8 browsers]: http://blog.jquery.com/2013/04/18/jquery-2-0-released/
[AngularJS 1.3 discontinues support for Internet Explorer 8]: http://angularjs.blogspot.jp/2013/12/angularjs-13-new-release-approaches.html
[Support for Windows XP ended April 8th, 2014]: https://www.microsoft.com/en-us/WindowsForBusiness/end-of-xp-support
[Bootstrap v4 dropped IE8 support]: http://blog.getbootstrap.com/2015/08/19/bootstrap-4-alpha/
[Support for older versions of Internet Explorer ended on January 12th, 2016]: https://www.microsoft.com/en-us/WindowsForBusiness/End-of-IE-support
[Discontinuing IE 8 Support in React DOM]: http://facebook.github.io/react/blog/2016/01/12/discontinuing-ie8-support.html
