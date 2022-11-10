# Maintainer: Ciaran Moran <25228551+morancj@users.noreply.github.com>
pkgname=aws-nuke
pkgver=2.20.0
pkgrel=1
pkgdesc="Nuke a whole AWS account and delete all its resources."
arch=(x86_64)
url="https://github.com/rebuy-de/aws-nuke"
license=('MIT')
depends=()
options=('!strip')
provides=('aws-nuke')
source=("${pkgname}-${pkgver}.tar.gz::${url}/releases/download/v${pkgver}/${pkgname}-v${pkgver}-linux-amd64.tar.gz")
sha512sums=('6b53c6ec3a523f67169f10790c3064597e2ea65bb4fe31e409c0e7cc1842dc3147591980c8d109466c90bb171b482266e5eef5579744136fab1ed62f328aa13f')

package() {
  mkdir -p "${pkgdir}/usr/bin"
  tar xzf "${pkgname}-${pkgver}.tar.gz"
  install -m755 "${srcdir}/${pkgname}-v${pkgver}-linux-amd64" "${pkgdir}/usr/bin/${pkgname}"
}

