# Maintainer: Florian Bruhin (The Compiler) <archlinux.org@the-compiler.org>

pkgname=drg2sbg
pkgver=2.2
pkgrel=2
pkgdesc="a tool to convert .drg files (I-Doser) to .sbg (SBaGen)"
arch=('i686' 'x86_64')
url="http://code.google.com/p/$pkgname/"
license=('GPL2')
source=("http://${pkgname}.googlecode.com/files/$pkgname-$pkgver.tar.gz")
sha1sums=('05a140e0832be6e41b7c7f76eff5d9e6295b2222')
depends=('glibc')

build() {
  cd "$pkgname-$pkgver"
  
  ./configure --prefix=/usr
  make
}

package() {
  cd "$srcdir/$pkgname-$pkgver"
  make DESTDIR="$pkgdir/" install
}

# vim:set ts=2 sw=2 et:
