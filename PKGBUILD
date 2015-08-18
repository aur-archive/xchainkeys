# Maintainer: Henning Bekel <h.bekel@googlemail.com>

pkgname=xchainkeys  
pkgver=0.11
pkgrel=1 
pkgdesc="Standalone keychains for X11"
url="http://henning-bekel.de/xchainkeys"
arch=('i686' 'x86_64')
license=('GPL3')
depends=('libx11')
source=(http://henning-bekel.de/download/$pkgname/$pkgname-$pkgver.tar.gz)
md5sums=('27c785c4517ae1c4cacd3c599404ecdb')

build() {
  cd "$srcdir/$pkgname-$pkgver"
  ./configure --prefix=/usr
  make 
}

package() {
  cd "$srcdir/$pkgname-$pkgver"
  make DESTDIR="$pkgdir" install
}
