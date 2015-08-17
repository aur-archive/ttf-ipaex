# Maintainer: ponsfoot <cabezon dot hashimoto at gmail dot com>

pkgname=ttf-ipaex
pkgver=001.03
_pkgver=${pkgver/./}
pkgrel=1
pkgdesc="Japanese outline fonts following the tradition of Japanese printing font"
arch=('any')
url="http://ossipedia.ipa.go.jp/ipafont/"
license=('custom')
depends=('fontconfig' 'xorg-font-utils')
install=ttf.install
changelog=ChangeLog
source=(http://info.openlab.ipa.go.jp/ipafont/fontdata/IPAexfont${_pkgver}.zip)

build() {
  cd ${srcdir}/IPAexfont${_pkgver}

  install -d ${pkgdir}/usr/share/fonts/TTF
  install -m644 *.ttf ${pkgdir}/usr/share/fonts/TTF/

  install -d ${pkgdir}/usr/share/licenses/${pkgname}
  install -m644 IPA_Font_License_Agreement_v1.0.txt Readme_IPAexfont${_pkgver}.txt \
                ${pkgdir}/usr/share/licenses/${pkgname}/
}

md5sums=('ac67b2fc3aab7f683d89f0070df284e7')
