

pkgname=axel
pkgver=2.4
pkgrel=1
pkgdesc="Download accelerator"
arch=('x86_64')
url="http://axel.alioth.debian.org/"
license=('GPL')
depends=('glibc')
source=(https://dev.archlinux.org/~foutrelis/sources/$pkgname/$pkgname-$pkgver.tar.gz)
sha256sums=('359a57ab4e354bcb6075430d977c59d33eb3e2f1415a811948fa8ae657ca8036')

build() {
  cd "$srcdir/$pkgname-$pkgver"

  ./configure --prefix=/usr
  make
}

package() {
  cd "$srcdir/$pkgname-$pkgver"
  make DESTDIR="$pkgdir" install
}

# vim:set ts=2 sw=2 et:
