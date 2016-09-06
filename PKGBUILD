pkgname='python3-markups'
pkgver=2.0.0
pkgrel=1
pkgdesc='Wrapper around various text markups'
arch=('x86_64')
url='https://launchpad.net/python-markups'
license=('BSD')
depends=('python3')
makedepends=('python3-setuptools')
source=($pkgname-$pkgver.tar.gz::http://github.com/retext-project/pymarkups/archive/$pkgver.tar.gz)
sha256sums=('0d1ac398ecde6ec3904ec842abee7538d58a3a2d51ac2e61584a822dc6d73a06')

package() {
  cd "${srcdir}"/pymarkups-$pkgver
  python3 setup.py install --root="${pkgdir}"
  install -Dm644 LICENSE "${pkgdir}"/usr/share/licenses/$pkgname/LICENSE
}
