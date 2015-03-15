Compiling

Compiling edb is generally quite simple. edb currently depends on the following packages:

  * [Qt](http://qt-project.org/) >= 4.6
  * [Boost](http://www.boost.org/) >= 1.35

Many distributions already have packages that satisfy these.

Once you have Qt installed, it is as simple as

```
$ qmake
$ make
```

This will build the debugger along with all plugins I have written. On certain systems your `qmake` make be named slightly differently, I've noticed that the Fedora Core rpms name it `qmake-qt4`.

If you are planning on doing a `make install`, you likely want to specify the default plugin path, here's how you would do that.

```
$ qmake -makefile DEFAULT_PLUGIN_PATH="/usr/lib/edb/"
$ make
```

For installation information, see [Installing](Installing.md)