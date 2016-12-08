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
sha256sums=('e9c8e8f0bd34474fe0474a809825d35761b7f21f1d2008c7455b82d8ab2624e9'
            '8dd8bbb0444f2043cce76ddd13db571296ec3cfb139a4c8be393a6b49202b31e')
