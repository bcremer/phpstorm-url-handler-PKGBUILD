phpstorm-url-handler
=============================

This [PKGBUILD](https://wiki.archlinux.org/index.php/PKGBUILD) provides a handler for the `pstorm://` URL schema to open a file in the [PhpStorm IDE](http://www.jetbrains.com/phpstorm/).

The following URL format is supported:

```bash
pstorm://open/?url=file://%f&line=%l
```

Example configuration for for [Xdebug](http://xdebug.org/):

```
xdebug.file_link_format="pstorm://open/?url=file://%f&line=%l"
```

Manual installation
-------

```
git clone https://github.com/bcremer/phpstorm-url-handler-PKGBUILD.git
cd phpstorm-url-handler-PKGBUILD
makepkg
sudo pacman -U phpstorm-url-handler-*.pkg.tar.xz
```


Credits
-------
The phpstorm-url-hander script is based on [aik099s](https://github.com/aik099) script used in [PhpStormProtocol](https://github.com/aik099/PhpStormProtocol).

The PKGBUILD is heavily inspired by [MrZYXs](https://github.com/MrZYX) [sublime-url-handler](https://github.com/MrZYX/PKGBUILDs/tree/master/sublime-url-handler).
