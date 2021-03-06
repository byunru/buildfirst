# Promise Basics

Promises are a big player in the asynchronous landscape, and a subject that can be tricky to understand. In section 6.3 of the book I demystify promises, and in this sample I'll present you with a bunch of examples of the most basic promises.

To test these out, you'll need either

- Visit [ES6 Fiddle][5], and paste the examples in there
- Get the [es6-promise][6] polyfill and try them out on your own
- Try them out in Chrome 32+, where Promises are enabled by default

```js
var promise = new Promise(function (resolve, reject) {
  if (Math.random() < 0.5) {
    resolve('Good enough.');
  } else {
    reject(new Error('Dice roll failed!'));
  }
});
```

Here's the complete list of examples you'll find in this sample.

- [Basic Promise][1]
- [Continuation][2] _(run a task when promise resolves)_
- [Asynchronous Promise][3] _(is just the same)_

![promises.png][4]

[1]: https://github.com/bevacqua/buildfirst/tree/master/ch06/08_promise_basics/01_basic.js
[2]: https://github.com/bevacqua/buildfirst/tree/master/ch06/08_promise_basics/02_thenable.js
[3]: https://github.com/bevacqua/buildfirst/tree/master/ch06/08_promise_basics/03_async-promise.js
[4]: https://raw.github.com/bevacqua/buildfirst/master/images/promises.png
[5]: http://www.es6fiddle.net/ "ES6 Fiddle Online"
[6]: https://github.com/jakearchibald/es6-promise "ES6 Promise Polyfill by Jake Archibald"
