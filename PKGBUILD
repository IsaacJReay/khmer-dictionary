pkgname=khmer-dictionary
pkgver=2.1
pkgrel=2

pkgdesc="Khmer Dictionary"

arch=('x86_64')
license=('MIT')

depends=('java-runtime')

source=(
    "${pkgname}-2.1.jar"
    "${pkgname}.desktop"
    "${pkgname}.png"
    "${pkgname}"
)
md5sums=(
    '229e40290617cf5c971d8ab9e58dff99'
    'a2ef08e0a59e57913ebd31d2e62537ab'
    'eec6ae98b54845083f3b9500c6aa1072'
    'fe4780ed57c8a3d23c039ae8e1cb4a47'
)

package() {
    install -Dm644 "${pkgname}.png" "${pkgdir}/usr/share/icons/${pkgname}.png"
    install -Dm644 "${pkgname}.desktop" "${pkgdir}/usr/share/applications/${pkgname}.desktop"
    install -Dm755 "${pkgname}-2.1.jar" "${pkgdir}/opt/khmer-dictionary/${pkgname}-2.1.jar"
    install -Dm755 "${pkgname}" "${pkgdir}/usr/bin/${pkgname}"    
}
