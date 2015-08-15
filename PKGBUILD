# Maintainer: Patrice Peterson <runiq at archlinux dot us>

pkgname=calibur
pkgver='20120117'
pkgrel=2
pkgdesc="A tool for clustering large numbers of protein decoys"
arch=('i686' 'x86_64')
url="http://calibur.sourceforge.net/"
license=('GPL')
source=(http://sourceforge.net/projects/$pkgname/files/$pkgname/Release-2012-01-17/$pkgname.tar.gz)
md5sums=('27d8d4040060275419fd3cdfd2638405')

build() {
  cd "$srcdir/$pkgname"
  make
}

package() {
  cd "$srcdir/$pkgname"
  install -d "$pkgdir/usr/bin"
  install -d "$pkgdir/usr/share/doc/calibur"

  install calibur "$pkgdir/usr/bin/calibur"
  install calibur-lite "$pkgdir/usr/bin/calibur-lite"
  install -m 644 README "$pkgdir/usr/share/doc/calibur/README"
}

# vim:set ts=2 sw=2 et:
