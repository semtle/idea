
[![idea](http://i.imgur.com/BGMt0Ne.png)](#)

# `$ idea`

 [![Support me on Patreon][badge_patreon]][patreon] [![Buy me a book][badge_amazon]][amazon] [![PayPal][badge_paypal_donate]][paypal-donations] [![Version](https://img.shields.io/npm/v/idea.svg)](https://www.npmjs.com/package/idea) [![Downloads](https://img.shields.io/npm/dt/idea.svg)](https://www.npmjs.com/package/idea)

> A lightweight CLI tool and module for keeping ideas in a safe place quick and easy.

## :cloud: Installation

You can install the package globally and use it as command line tool:


```sh
$ npm i -g idea
```


Then, run `idea --help` and see what the CLI tool can do.


```
$ idea --help
idea help
usage: idea [command] <idea|filter|id>

A lightweight CLI tool and module for keeping your ideas in a safe place quick and easy.

[command]
  create <idea>           Creates and saves a new idea. Example: `idea create "Implement something very cool"`
  list                    Lists all ideas. Example: `idea list`
  filter <filter>         Lists filtered ideas. Example: `idea filter '{"state": "SOLVED"}'`
  solve <id>              Solves an idea. Example `idea solve 1`
  help                    Prints this help.

Documentation can be found at https://github.com/IonicaBizau/idea
```

## :clipboard: Example


Here is an example how to use this package as library. To install it locally, as library, you can do that using `npm`:

```sh
$ npm i --save idea
```



```js
// Dependencies
var Idea = require("idea");

// Initialize the idea object
var idea = new Idea("./ideas.json", err => {
    if (err) throw err;
    idea.create("Implement something cool.", err => {
        if (err) throw err;
    });
});
```

## :question: Get Help

There are few ways to get help:

 1. Please [post questions on Stack Overflow](https://stackoverflow.com/questions/ask). You can open issues with questions, as long you add a link to your Stack Overflow question.
 2. For bug reports and feature requests, open issues. :bug:
 3. For direct and quick help from me, you can [use Codementor](https://www.codementor.io/johnnyb). :rocket:


## :memo: Documentation

For full API reference, see the [DOCUMENTATION.md][docs] file.

## :yum: How to contribute
Have an idea? Found a bug? See [how to contribute][contributing].


## :sparkling_heart: Support my projects

I open-source almost everything I can, and I try to reply everyone needing help using these projects. Obviously,
this takes time. You can integrate and use these projects in your applications *for free*! You can even change the source code and redistribute (even resell it).

However, if you get some profit from this or just want to encourage me to continue creating stuff, there are few ways you can do it:

 - Starring and sharing the projects you like :rocket:
 - [![PayPal][badge_paypal]][paypal-donations]—You can make one-time donations via PayPal. I'll probably buy a ~~coffee~~ tea. :tea:
 - [![Support me on Patreon][badge_patreon]][patreon]—Set up a recurring monthly donation and you will get interesting news about what I'm doing (things that I don't share with everyone).
 - **Bitcoin**—You can send me bitcoins at this address (or scanning the code below): `1P9BRsmazNQcuyTxEqveUsnf5CERdq35V6`

    ![](https://i.imgur.com/z6OQI95.png)

Thanks! :heart:



## :scroll: License

[MIT][license] © [Ionică Bizău][website]

[badge_patreon]: http://ionicabizau.github.io/badges/patreon.svg
[badge_amazon]: http://ionicabizau.github.io/badges/amazon.svg
[badge_paypal]: http://ionicabizau.github.io/badges/paypal.svg
[badge_paypal_donate]: http://ionicabizau.github.io/badges/paypal_donate.svg
[patreon]: https://www.patreon.com/ionicabizau
[amazon]: http://amzn.eu/hRo9sIZ
[paypal-donations]: https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=RVXDDLKKLQRJW
[donate-now]: http://i.imgur.com/6cMbHOC.png

[license]: http://showalicense.com/?fullname=Ionic%C4%83%20Biz%C4%83u%20%3Cbizauionica%40gmail.com%3E%20(https%3A%2F%2Fionicabizau.net)&year=2015#license-mit
[website]: https://ionicabizau.net
[contributing]: /CONTRIBUTING.md
[docs]: /DOCUMENTATION.md
