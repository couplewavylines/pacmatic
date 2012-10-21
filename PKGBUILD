# $Id: PKGBUILD 78601 2012-10-21 20:40:13Z kkeen $
# Maintainer: Kyle Keen <keenerd@gmail.com>
pkgname=pacmatic
pkgver=20121021
pkgrel=1
pkgdesc="A pacman wrapper to avoid bricking your system and such other surprises."
arch=('any')
url="http://kmkeen.com/pacmatic/"
license=('GPL')
depends=('pacman' 'bash' 'pacman-contrib' 'expac')
makedepends=()
optdepends=('vim: for vimdiff'
            'html2text: for prettier news')
source=(http://kmkeen.com/pacmatic/$pkgname-$pkgver.tar.gz)
md5sums=('6076fc923c0fc215c3dbe06e06f7405a')

package() {
  cd "$srcdir/$pkgname"
  install -D -m 0755 $pkgname      "$pkgdir/usr/bin/$pkgname"
  install -D -m 0755 cron-$pkgname "$pkgdir/usr/bin/cron-$pkgname"
  install -D -m 0644 $pkgname.1    "$pkgdir/usr/share/man/man1/$pkgname.1"
}

