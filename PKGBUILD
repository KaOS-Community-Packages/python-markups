pkgname=python-markups
_pkgbasename=pymarkups
pkgver=3.1.1
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
sha256sums=('62055078b8e10fbe6470e9cf57aa40299462c87102649817d26ae6c5d4831505')

package() {
	cd "${_pkgbasename}-${pkgver}"
	python3 setup.py install --root="${pkgdir}"
	install -Dm644 LICENSE "${pkgdir}"/usr/share/licenses/$pkgname/LICENSE
}
