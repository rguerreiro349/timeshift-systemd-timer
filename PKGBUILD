#
# Contribuidor: {{ nome_do_autor(); }}
#

pkgname=timeshift-systemd-timer
pkgver=0.0.1
pkgrel=2
pkgdesc="Adicionar suporte systemd para timeshift"
arch=("any")
license=("cIO")
depends=('systemd' 'timeshift')
source=(
    local://timeshift-boot.service
    local://timeshift-boot.timer
    local://timeshift-hourly.service
    local://timeshift-hourly.timer
)
sha256sums=('SKIP'
    'SKIP'
    'SKIP'
    'SKIP')

package()
{
    install -m755 -d "${pkgdir}/usr/lib/systemd/system"
    install -m644 ${srcdir}/* ${pkgdir}/usr/lib/systemd/system
}
