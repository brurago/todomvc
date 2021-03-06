# Dart TodoMVC Example

> Dart is a class-based, object-oriented language with lexical scoping,
> closures, and optional static typing. Dart helps you build structured modern
> web apps and is easy to learn for a wide range of developers.

> _[Dart - dartlang.org][dart]_

This version of TodoMVC is a "vanilla" Dart implementation. The
core [Dart SDK][sdk] is required. No web frameworks are used. However,
this implementation uses two packages from the [pub package repository][pub].

# Running the app

Simply open the `build/index.html` file in your favorite modern browser. We
have taken the liberty of pre-compiling the Dart app into JavaScript for you.

# Directory layout

This app follows the [pub package layout conventions][pkglayout].

`build` - the pre-built example, ready to run in any modern browser. This
  directory is generated by the build system. Do not modify files in this
  directory.

`pubspec.yaml` - project metadata and a list of dependencies.

`lib` - Dart code, such as models.

`web` - web resources, such as HTML and CSS.

`web/dart` - Dart code specific to this web app.

# Editing and rebuilding

If you want to make changes to the app, follow these instructions. For very
fast development cycles, we recommend using [Dartium][] (a
custom build of Chromium with an embedded Dart VM). With Dartium, you can
simply reload the Dart code to instantly see your changes. However, you
need to run `pub build` to prep the app for browsers without Dart VM.

## Installing the SDK

First, download [Dart Editor][editor] (which includes the Dart SDK)
or the [Dart SDK][sdk]. Put the SDK's bin directory on your PATH.

## Installing packages

Dart Editor automatically runs Dart's package manager to install
package dependencies. If you did not open the project in Dart Editor,
you need to manually install the dependencies:

```
cd vanilla-examples/vanilladart
pub get
```

## Building the app

You need to compile the app into JavaScript to run in your browser.

```
cd vanilla-examples/vanilladart
pub build
```

The above command creates a `build` directory, complete with HTML files
and a compiled-to-JavaScript version of the app.

# Learning Dart

The [Dart website][dart] is a great resource for learning
Dart.

Getting started:

* [Try Dart](https://www.dartlang.org/codelabs/darrrt/)

Here are some links you may find helpful:

* [API Reference](https://api.dartlang.org/)
* [A Tour of the Dart Language][langtour]
* [Articles](http://www.dartlang.org/articles)
* [Tutorials](http://www.dartlang.org/docs/tutorials)
* [FAQ](http://www.dartlang.org/support/faq.html)

Get help from other Dart users:

* [Dart on StackOverflow](http://stackoverflow.com/questions/tagged/dart)
* [Support](https://www.dartlang.org/support/)

Follow the Dart project:

* [Dart on Twitter](http://twitter.com/dart_lang)
* [Dart on Google +](https://plus.google.com/+dartlang/posts)

_If you have other helpful links to share, or find any of the links above no
longer work, please [let us know](https://github.com/tastejs/todomvc/issues)._

[![Build Status](https://drone.io/mlorber/todomvc-dart/status.png)][buildstatus]

Build history can be seen [here][builds].


## Credit

This TodoMVC application was created by [Mathieu Lorber](http://mlorber.net).

[langtour]: http://www.dartlang.org/docs/dart-up-and-running/contents/ch02.html
[dart]: https://www.dartlang.org
[builds]: https://drone.io/mlorber/todomvc-dart
[buildstatus]: https://drone.io/mlorber/todomvc-dart/latest
[sdk]: https://www.dartlang.org/tools/sdk/
[pub]: http://pub.dartlang.org
[editor]: https://www.dartlang.org/tools/editor/
[pkglayout]: http://pub.dartlang.org/doc/package-layout.html
[Dartium]: https://www.dartlang.org/tools/dartium/