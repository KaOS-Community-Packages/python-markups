pkgname=python-markups
_pkgbasename=pymarkups
pkgver=3.1.3
pkgrel=1
pkgdesc='Wrapper around various text markups'
arch=('x86_64')
url='https://launchpad.net/python-markups'
license=('BSD')
depends=('python3')
makedepends=('python3-setuptools')
provides=('python3-markups')
replaces=('python3-markups')
conflicts=('python3-markups')
source=("http://github.com/retext-project/${_pkgbasename}/archive/${pkgver}.tar.gz")
sha256sums=('c6982db63675313464fe00bb9c35ae98dc0a20c59ecb387d19cfeb6f427cee10')

package() {
	cd "${_pkgbasename}-${pkgver}"
	python3 setup.py install --root="${pkgdir}"
	install -Dm644 LICENSE "${pkgdir}"/usr/share/licenses/$pkgname/LICENSE
}
