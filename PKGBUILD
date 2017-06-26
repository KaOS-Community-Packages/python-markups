pkgname='python3-markups'
pkgver=2.0.1
pkgrel=1
pkgdesc='Wrapper around various text markups'
arch=('x86_64')
url='https://launchpad.net/python-markups'
license=('BSD')
depends=('python3')
makedepends=('python3-setuptools')
source=($pkgname-$pkgver.tar.gz::http://github.com/retext-project/pymarkups/archive/$pkgver.tar.gz)
sha256sums=('c12b8b3b1dc8bc731dff01d0470718aea46338e9e44c65b9006e6fb0100e716a')

package() {
  cd "${srcdir}"/pymarkups-$pkgver
  python3 setup.py install --root="${pkgdir}"
  install -Dm644 LICENSE "${pkgdir}"/usr/share/licenses/$pkgname/LICENSE
}
