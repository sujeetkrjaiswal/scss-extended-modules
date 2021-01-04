# scss-extended-modules

> This package has been moved from `scss-extended-modules` to `@scss-toolkit/extended-modules`

This provides functions built on top of built-in modules `sass:<modules>`.

## Motivation

When working with SCSS/SASS, most of the time we stick with features like mixins, nested selector and re-usable variables.
But when we need to create configurable and extensible libraries; programming capabilities help reduce lines of code and hence
possibility of bugs.

Sass Commes with its own built-in modules with limited set of functions. This package tries to extends those functionalities
with functions similar to `javascript in-built functions` for `list`, `maps`, etc.

The main reason for choosing to provide functions similar to javascript, is that most of the front-end engineers will be more
familier with javascript as compared to any other language.

## Supported Extended modules

| Extended modules | Extends built-in module | Methods                                                    |
| ---------------- | ----------------------- | ---------------------------------------------------------- |
| elist            | sass:list               | is, is-non-empty, join-all, find, some, every, filter      |
| emap             | sass:map                | new, is, is-non-empty, merge-all, set                      |
| emath            | sass:math               | sign, mod, js-mod, is-even, is-odd, pow-series             |
| emeta            | sass:meta               |
| eselector        | sass:selector           | is-classname-selector                                      |
| estring          | sass:string             | is, is-non-empty, repeat, join-all, starts-with, ends-with |

## Supported Sass implementation

**Dart Sass**

- Node Sass is several years behind Dart Sass and the official Sass specification.
- LibSass and packages built on top of it (e.g: Node Sass) is officially deprecated. ([Deprecation Notice](https://sass-lang.com/blog/libsass-is-deprecated), [Github Issue](https://github.com/sass/node-sass/issues/2952))
- Dart Sass supports [Module System](https://sass-lang.com/blog/the-module-system-is-launched)

[Read more on Why we stick with dart-sass](https://scss-toolkit.github.io/why-dart-sass)
