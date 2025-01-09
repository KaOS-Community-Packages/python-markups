pkgname=python-markups
_pkgbasename=pymarkups
pkgver=4.1.0
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
sha256sums=('2e51aa1511336f2ab0575f42e0f1aecdba04ec9793eb82f791aa285982a53920')

build() {
	cd "${_pkgbasename}-${pkgver}"
	python3 -m build --wheel
}

package() {
	cd "${_pkgbasename}-${pkgver}"
	python3 -m installer --destdir="${pkgdir}" dist/*.whl
	install -Dm644 LICENSE "${pkgdir}"/usr/share/licenses/$pkgname/LICENSE
}
