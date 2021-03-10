# Maintainer: Ciaran Moran <25228551+morancj@users.noreply.github.com>
pkgname=aws-nuke
pkgver=2.14.0
pkgrel=1
pkgdesc="Nuke a whole AWS account and delete all its resources."
arch=(x86_64)
url="https://github.com/rebuy-de/aws-nuke"
license=('MIT')
depends=()
options=('!strip')
provides=('aws-nuke')
source=("${pkgname}-${pkgver}.tar.gz::${url}/releases/download/v${pkgver}/${pkgname}-v${pkgver}-linux-amd64.tar.gz")
sha512sums=('166fbcab3a4b8077b599e7aaecf95157dc313846d1fe616f6726af41c50b562074efe72c32609a077a3731eb10ba61d726420a896b9d419f38c534a9bb35b87a')

package() {
  mkdir -p "${pkgdir}/usr/bin"
  tar xzf "${pkgname}-${pkgver}.tar.gz"
  install -m755 "${srcdir}/dist/${pkgname}-v${pkgver}-linux-amd64" "${pkgdir}/usr/bin/${pkgname}"
}

