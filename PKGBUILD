# Maintainer: Erik Dubois <erik.dubois@gmail.com>
pkgname=carli-5-calamares-config-dev
_pkgname=carli-5-calamares-config-dev
_destname="/etc/calamares"
pkgver=21.02
pkgrel=1
pkgdesc="calamares for carli arcolinux"
arch=('any')
url="https://github.com/arcolinux/${_pkgname}"
license=('GPL3')
makedepends=('git')
depends=()
conflicts=()
provides=("${pkgname}")
options=(!strip !emptydirs)
source=(${_pkgname}::"git+${url/${_pkgname}.git")
sha256sums=('SKIP')
package() {
	mkdir -p "${pkgdir}${_destname}"
	cp -r "${srcdir}/${_pkgname}/calamares/"* "${pkgdir}${_destname}"
}