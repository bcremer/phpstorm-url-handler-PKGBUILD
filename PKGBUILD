# Maintainer: Benjamin Cremer <bc@benjamin-cremer.de>

pkgname=phpstorm-url-handler
pkgver=0.0.1
pkgrel=1
pkgdesc="Open pstorm:// URLs in phpstorm. Based on http://blog.byscripts.info/2013/02/txmt-protocol-and-sublime-text-2-english.html"
url='https://github.com/bcremer/phpstorm-url-handler-PKGBUILD'
arch=('any')
license=('MIT')
depends=('desktop-file-utils')
install=phpstorm-url-handler.install
source=($pkgname $pkgname.desktop)

package() {
  install -Dm755 $pkgname         "$pkgdir/usr/bin/$pkgname"
  RPM_BUILD_ROOT=$pkgdir desktop-file-install $pkgname.desktop
}

# vim:set ts=2 sw=2 et:
sha256sums=('46c4f60312cd31b5c6f27310542879bc3f3bb0bf432715ef2d14781cda7a125f'
            '8dd8bbb0444f2043cce76ddd13db571296ec3cfb139a4c8be393a6b49202b31e')
