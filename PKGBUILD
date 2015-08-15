# Contributor: Kevin Piche <kevin@archlinux.org>
# Contributor: Sarah Hay <sarahhay@mb.sympatico.ca>

pkgname=gift-openft
pkgver=0.2.1.6
pkgrel=10
pkgdesc="GiFT's OpenFT plugin"
arch=('i686' 'x86_64')
url="http://gift.sourceforge.net/"
license=('GPL')
depends=('gift' 'zlib' 'db')
source=(http://downloads.sourceforge.net/sourceforge/gift/$pkgname-$pkgver.tar.bz2)
md5sums=('6661f01304246a29aeabda113691ca93')

build() {
  cd $srcdir/$pkgname-$pkgver
  ./configure --prefix=/usr
  make 
}

package() {
  cd $srcdir/$pkgname-$pkgver
  make DESTDIR=$pkgdir install 
} 
