# Maintainer: Ciaran Moran <25228551+morancj@users.noreply.github.com>
pkgname=aws-nuke
pkgver=2.15.0
pkgrel=1
pkgdesc="Nuke a whole AWS account and delete all its resources."
arch=(x86_64)
url="https://github.com/rebuy-de/aws-nuke"
license=('MIT')
depends=()
options=('!strip')
provides=('aws-nuke')
source=("${pkgname}-${pkgver}.tar.gz::${url}/releases/download/v${pkgver}/${pkgname}-v${pkgver}-linux-amd64.tar.gz")
sha512sums=('f21b07577954067b2a5fda54ebdb7dcef33b342a200ee65e7ebf9e95567ff7c0ef4c47f50f17410d690eb03dee6d40a822ca546f27659ef24e43e560915e2e82')

package() {
  mkdir -p "${pkgdir}/usr/bin"
  tar xzf "${pkgname}-${pkgver}.tar.gz"
  install -m755 "${srcdir}/${pkgname}-v${pkgver}-linux-amd64" "${pkgdir}/usr/bin/${pkgname}"
}

