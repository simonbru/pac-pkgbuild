# Maintainer: Ricardo Band <email@ricardo.band>
pkgname=pac-simonbru
provides=(pac)
conflicts=(pac)
pkgver=1.3.6
pkgrel=1
pkgdesc="Small wrapper around pacaur to mimic yaourts search feature (simonbru's fork)"
arch=(any)
url="https://github.com/simonbru/pac"
license=('MIT')
depends=('python>=3.6.0'
         'pacaur')
source=("https://github.com/simonbru/pac/archive/v${pkgver}.tar.gz"
        "https://github.com/simonbru/pac/releases/download/v${pkgver}/v${pkgver}.tar.gz.asc")
validpgpkeys=('D67115C4621A58260F3C181B4151AA35EEEE1E46')  # Simon Brulhart
sha256sums=('b3c85a63cb94d35aa3d266457570eeef24d0f8300ee320f853c13cbd884228da'
            'SKIP')

package() {
    install -dm 755 "$pkgdir"/usr/bin/
    install -m 755 "pac-${pkgver}/pac" "$pkgdir"/usr/bin/
}
