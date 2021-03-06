---
permalink: /
title: Introduction
---
This exercise will walk you through writing a small
[Node.js](https://nodejs.org/) application and writing unit tests for it. You
will learn how to:

- Structure your code to separate concerns effectively, which maximizes
  readability, maintainability, and testability
- Write small, focused tests for your application-specific logic
- Use a technique known as "dependency injection" to simulate interaction with
  a remote service
- Write an automated integration test for your application

## Assumptions

This exercise assumes you're comfortable executing commands in a UNIX
environment. Specifically, it expects that you're familiar with the basics of
how to create directories and files on the command line of a terminal program.

This exercise also assumes that you have already installed Node.js version 4.2
or greater and Ruby version 2.2.3 or greater. See the [Installation section of
the README][installation] for instructions on how to set up Node.js and Ruby
development environments.

[installation]: https://github.com/mbland/slack-github-issues#Installation

**OS X users**: Consider using [Homebrew](http://brew.sh/) to install this
software.

### Why do we need to install Ruby? Isn't this a Node.js exercise?

The `./go` script to build the site and run other commands for the exercise is
written in Ruby. The exercise content is published and hosted on `localhost`
using [Jekyll](https://jekyllrb.com/), a Ruby application.

## Tools

The tests will use:

- [Mocha test framework](https://mochajs.org/)
- [Chai assertion library](http://chaijs.com/), specifically the [Chai
  Behavior-Driven Development style assertions](http://chaijs.com/api/bdd/).
- [Sinon spy, stub, and mock object library](http://sinonjs.org/)

Also, the code will make use of the [Promise
type](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise),
standard in JavaScript/ECMAScript 6 and Node.js versions 0.12.7 and up.
Promises are the standard way to write asynchronous operations. This exercise
will try to introduce you to their effective use (and to avoid some of the
pitfalls!).
