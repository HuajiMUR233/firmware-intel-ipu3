# Maintainer: Nek0U <neko@jvav.me>

pkgname=firmware-intel-ipu3
pkgver=1.0.0
pkgrel=1
pkgdesc="Intel IPU3 firmware"
arch=('any')
url="https://git.kernel.org/pub/scm/linux/kernel/git/firmware/linux-firmware.git"
license=("custom")
source=(
    "https://git.kernel.org/pub/scm/linux/kernel/git/firmware/linux-firmware.git/plain/intel/ipu/irci_irci_ecr-master_20161208_0213_20170112_1500.bin"
    "https://git.kernel.org/pub/scm/linux/kernel/git/firmware/linux-firmware.git/plain/LICENSE.ipu3_firmware"
)
sha256sums=(
    "f538714042e694b0e13eedea6a84bfe9b2c94416c0031f6a1a3e8a7cedb29b7c"
    "22324f462d5c82e0ea4e265413af7b019454e478112822d21ed0c65eb3cb3cc2"
)
package() {
    install -Dm644 irci_irci_ecr-master_20161208_0213_20170112_1500.bin "${pkgdir}/usr/lib/firmware/intel/ipu3-fw.bin"
    install -Dm644 LICENSE.ipu3_firmware "${pkgdir}/usr/share/licenses/$pkgname/LICENSE.ipu3_firmware"
}
