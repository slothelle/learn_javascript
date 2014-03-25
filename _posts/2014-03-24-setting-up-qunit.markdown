---
layout: post
title:  "Setting up Qunit"
date:   2014-03-24 14:54:53
categories: week1
tags: javascript testing qunit
---

Qunit is a very easy way to write tests for your JavaScript. All of the JavaScript you write should be tested.

JSBin allows you to easily add Qunit into any project (click 'Add library' and select Qunit). [Here is a sample project](http://jsbin.com/cixal/2/edit?html,js,output) with a few additional tweaks added to make the output a little bit prettier.

<a class="jsbin-embed" href="http://jsbin.com/cixal/2/embed?html,js,output&height=600px">QUnit</a><script src="http://static.jsbin.com/js/embed.js" height="800px"></script>

Your tests will run automatically as you type. If this is distracting, hide the output panel while you're working by click 'Output' at the top of the screen.

The Qunit assertion API is really small, you only have to learn a few methods. An `assertion` is when you're stating that you believe object A == object B. You can also use negative associations, that assert the two objects don't match.

Definitely read about the different asssertion types before you try and write any tests.

**Required reading**

* [Qunit assertion API](https://api.qunitjs.com/category/assert/)
* [Qunit `module`](https://api.qunitjs.com/module/) for organizing your tests into groups
* [Qunit `test`](https://api.qunitjs.com/test/)

Assertions that expect objects to match include:

* `deepEqual(thing1, thing2, 'Optional test message');`
* `equal(thing1, thing2, 'Optional test message');`
* `ok(thing1, thing2, 'Optional test message');`
* `propEqual(thing1, thing2, 'Optional test message');`
* `strictEqual(thing1, thing2, 'Optional test message');`

Assertions that expect objects to NOT match include:

* `notDeepEqual(thing1, thing2, 'Optional test message');`
* `notEqual(thing1, thing2, 'Optional test message');`
* `notPropEqual(thing1, thing2, 'Optional test message');`
* `notStrictEqual(thing1, thing2, 'Optional test message');`

Assertions that expect errors:

* `throws(callback);` - Don't worry about this for now, just know that it is here.