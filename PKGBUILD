# Maintainer: Nuno Araujo <nuno.araujo at russo79.com>
pkgname=python2-pylibg19
_pkgname=pylibg19
pkgver=0.0.7
pkgrel=1
pkgdesc="Basis for G19 support in Gnome15"
arch=(any)
url="http://www.russo79.com/gnome15"
license=('GPL')
depends=(python2 python2-pyusb python2-imaging)
conflicts=('pylibg19')
replaces=('pylibg19')
source=(https://projects.russo79.com/attachments/download/126/${_pkgname}-${pkgver}.tar.gz)
md5sums=('a680a7ddc54e04f244b599776bd74a46')

build() {
  cd "${srcdir}/${_pkgname}-${pkgver}"
  python2 setup.py build
}

package() {
  cd "${srcdir}/${_pkgname}-${pkgver}"
  python2 setup.py install --prefix='/usr' --root=${pkgdir}
}

# vim:set ts=2 sw=2 et:
