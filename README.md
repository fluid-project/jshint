JSHint - Fluid Project Edition
==============================

This repository contains the Fluid Project's version of the JSHint JavaScript linting tool.

This version was forked from the main jshint project at its revision [`bf886b8f07124ddfbef158d7269e7b3b184a65fe`](https://github.com/jshint/jshint/commit/bf886b8f07124ddfbef158d7269e7b3b184a65fe)
of Tue Mar 25 23:01:58 2014 -0700, which occurred shortly after the release of its 2.4.4 version, and before the
release of its 2.5.0 version. Following that revision, all support for whitespace-based linting was removed
from jshint.

As well as retaining all features as of that revision, this version of the project includes the following
extra facilities:

 * When the `trailing:true` option is enabled, all lines containing trailing whitespace are flagged, including those that are otherwise blank or comment lines
 * A new option `mulopwhite:true` can be enabled, which permits whitespace to be lax around multiplicative operators, allowing constructions like `2*x + 3*y` to be permissible
 * The `jshint:ignore` directive (as well as all other jshint: directives) now is more permissive in allowing arbitrary material to follow in the comment line after whitespace - 
this allows one-line `jshint:ignore` comments to be annotated on the same line to provide a human-readable reason for why the ignore directive is there 

The original README file from the JSHint project's forked revision appears below (note that after many years the promised JSHint 3 rewrite has not arrived):


JSHint, A Static Code Analysis Tool for JavaScript
--------------------------------------------------

\[ [Use it online](http://jshint.com/) •  [About](http://jshint.com/about/) •
[Docs](http://jshint.com/docs/) • [FAQ](http://jshint.com/docs/faq) •
[Install](http://jshint.com/install/) • [Hack](http://jshint.com/hack/) •
[Blog](http://jshint.com/blog/) • [Twitter](https://twitter.com/jshint/) \]

[![Build Status](https://travis-ci.org/jshint/jshint.png?branch=2.x)](https://travis-ci.org/jshint/jshint)
[![NPM version](https://badge.fury.io/js/jshint.png)](http://badge.fury.io/js/jshint)

JSHint is a community-driven tool to detect errors and potential problems
in JavaScript code and to enforce your team’s coding conventions. It is
very flexible so you can easily adjust it to your particular coding guidelines
and the environment you expect your code to execute in.

#### JSHint 2.x versus JSHint 3

There's an effort going on to release the next major version of JSHint. All
development in the `master` branch is for the version 3.0. Current stable
version is in the `2.x` branch. Keep that in mind when submitting pull requests.

Also, before reporting a bug or thinking about hacking on JSHint, read this:
[JSHint 3 plans](http://www.jshint.com/blog/jshint-3-plans/). TL;DR: we're
moving away from style checks within JSHint so no new features around
style checks will be accepted. Bug fixes are fine for the `2.x` branch.

#### Reporting a bug

To report a bug simply create a
[new GitHub Issue](https://github.com/jshint/jshint/issues/new) and describe
your problem or suggestion. We welcome all kind of feedback regarding
JSHint including but not limited to:

 * When JSHint doesn't work as expected
 * When JSHint complains about valid JavaScript code that works in all browsers
 * When you simply want a new option or feature

Before reporting a bug look around to see if there are any open or closed tickets
that cover your issue. And remember the wisdom: pull request > bug report > tweet.


#### License

JSHint is distributed under the MIT License. One file and one file only
(src/stable/jshint.js) is distributed under the slightly modified MIT License.


#### Thank you!

We really appreciate all kind of feedback and contributions. Thanks for using and supporting JSHint!
