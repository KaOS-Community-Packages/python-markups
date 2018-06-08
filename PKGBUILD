pkgname='python3-markups'
pkgver=3.0.0
pkgrel=1
pkgdesc='Wrapper around various text markups'
arch=('x86_64')
url='https://launchpad.net/python-markups'
license=('BSD')
depends=('python3')
makedepends=('python3-setuptools')
source=($pkgname-$pkgver.tar.gz::http://github.com/retext-project/pymarkups/archive/$pkgver.tar.gz)
sha256sums=('5edc73ceed7d5ee207c481cc67852b5e54c731d65a32cb06afc27c455d5e70f4')

package() {
  cd "${srcdir}"/pymarkups-$pkgver
  python3 setup.py install --root="${pkgdir}"
  install -Dm644 LICENSE "${pkgdir}"/usr/share/licenses/$pkgname/LICENSE
}
