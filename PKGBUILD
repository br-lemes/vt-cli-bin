# Maintainer: Breno Ramalho Lemes <breno@br-lemes.net>
pkgname=vt-cli-bin
pkgver=1.3.1
pkgrel=1
pkgdesc='VirusTotal Command Line Interface'
arch=('x86_64')
url='https://github.com/VirusTotal/vt-cli'
license=('Apache-2.0')
provides=('vt-cli')
conflicts=('vt-cli')
depends=('glibc')
options=('!debug')
source=(
	"Linux64-${pkgver}.zip::${url}/releases/download/${pkgver//_/-}/Linux64.zip"
	"${url}/raw/refs/heads/master/LICENSE"
)
sha256sums=(
	'a340bcb2ee98aff6f19bde1de30702ddf106cbbc63b4309f60b33058e7689266'
	'cfc7749b96f63bd31c3c42b5c471bf756814053e847c10f3eb003417bc523d30'
)

package() {
	install -Dm755 "${srcdir}/vt" "${pkgdir}/usr/bin/vt"
	install -Dm644 LICENSE -t "${pkgdir}/usr/share/licenses/${pkgname}"
}
