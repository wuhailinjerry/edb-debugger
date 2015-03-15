# Installing #

Basic installation is simple, you may run

```
$ make install
```

Or if you would like to specify where things should go, you probably want to use something like this
```
$ make INSTALL_ROOT=/usr/ install
```

In which case the plugins will be installed in `/usr/lib/edb` and the binaries will be installed in `/usr/bin/`. Finally, if you are doing a `make install`, you probably want to specify a default plugin path, this is done during the `qmake` process, see [Compiling](Compiling.md).