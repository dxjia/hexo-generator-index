# hexo-generator-index

[![Build Status](https://travis-ci.org/hexojs/hexo-generator-index.svg?branch=master)](https://travis-ci.org/hexojs/hexo-generator-index)  [![NPM version](https://badge.fury.io/js/hexo-generator-index.svg)](http://badge.fury.io/js/hexo-generator-index) [![Coverage Status](https://img.shields.io/coveralls/hexojs/hexo-generator-index.svg)](https://coveralls.io/r/hexojs/hexo-generator-index?branch=master)

Index generator for [Hexo].

## Installation

``` bash
$ npm install hexo-generator-index --save
```

## Options

``` yaml
index_generator:
  per_page: 10
  order_by: -date
```

- **per_page**: Posts displayed per page. (0 = disable pagination)
- **order_by**: Posts order. (Order by date descending by default)

## Support Articles Stick Function
Reference : [解决Hexo置顶问题](http://www.netcan666.com/2015/11/22/%E8%A7%A3%E5%86%B3Hexo%E7%BD%AE%E9%A1%B6%E9%97%AE%E9%A2%98/)
在原作者基础上增加文章置顶功能，使用方法：
- 使用 替换你的 `node_modules/hexo-generator-index/lib/generator.js`；
- 在写文章时，在文章顶部的format里增加top属性，值越大，置顶越靠前；不写的代表不置顶；
```
title: Hello World
date: 2016-01-26 19:28:45
top: 10
---
```

## License

MIT

[Hexo]: http://hexo.io/
