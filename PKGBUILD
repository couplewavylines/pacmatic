# $Id: PKGBUILD 79784 2012-11-12 14:45:33Z kkeen $
# Maintainer: Kyle Keen <keenerd@gmail.com>
pkgname=pacmatic
pkgver=20121112
pkgrel=1
pkgdesc="A pacman wrapper to avoid bricking your system and such other surprises."
arch=('any')
url="http://kmkeen.com/pacmatic/"
license=('GPL')
depends=('pacman' 'bash' 'pacman-contrib' 'expac')
makedepends=()
optdepends=('vim: for vimdiff'
            'html2text: for prettier news')
source=(http://kmkeen.com/$pkgname/$pkgname-$pkgver.tar.gz)
md5sums=('200a0bda1f1bff73f152517f39b1be2e')

package() {
  cd "$srcdir/$pkgname"
  install -D -m 0755 $pkgname      "$pkgdir/usr/bin/$pkgname"
  install -D -m 0755 cron-$pkgname "$pkgdir/usr/bin/cron-$pkgname"
  install -D -m 0644 $pkgname.1    "$pkgdir/usr/share/man/man1/$pkgname.1"
}

