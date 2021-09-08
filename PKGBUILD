pkgname=python-markups
_pkgbasename=pymarkups
pkgver=3.1.2
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
sha256sums=('011df506e3f6a3afbf0294771ba025fc36f1969d7c4290cbdc71c437e9928afd')

package() {
	cd "${_pkgbasename}-${pkgver}"
	python3 setup.py install --root="${pkgdir}"
	install -Dm644 LICENSE "${pkgdir}"/usr/share/licenses/$pkgname/LICENSE
}
