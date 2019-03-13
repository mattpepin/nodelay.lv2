# Maintainer: David Runge <dave@sleepmap.de>
# Contributor: Lieven Moors <lievenmoors@gmail.com>

pkgname=nodelay-stereo
pkgver=20190206
pkgrel=1
pkgdesc="nodelaystereo LV2 plugin"
arch=('x86_64')
url="https://github.com/mattpepin/nodelay.lv2"
license=('GPL')
depends=('jack')
makedepends=('lv2')
groups=('lv2-plugins' 'pro-audio')
source=(${pkgname}-${pkgver}::"git+https://github.com/mattpepin/nodelay.lv2")
md5sums=('SKIP')

build() {
  cd "${pkgname}-${pkgver}"
  make
}

package() {
  cd "${pkgname}-${pkgver}"
  make install DESTDIR="$pkgdir/" PREFIX=/usr
}

# vim:set ts=2 sw=2 et:
