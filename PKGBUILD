# Maintainer: Robert Mackanics <schnoopay@gmail.com>

pkgname="libreoffice-en-us-help"
pkgver=4.2.6
pkgrel=1
pkgdesc="en-US offline help for Libreoffice"
arch=('any')
url="http://www.documentfoundation.org"
license=('LGPL')
makedepends=('rpmextract')
conflicts=('libreoffice-fresh-en-us-help')
source=("http://download.documentfoundation.org/libreoffice/stable/${pkgver}/rpm/x86/LibreOffice_${pkgver}_Linux_x86_rpm_helppack_en-US.tar.gz")

prepare() {
rpmextract.sh ${srcdir}/LibreOffice_$pkgver*_Linux_x86_rpm_helppack_en-US/RPMS/*.rpm
}

package() {
  mkdir -p "$pkgdir"/usr/lib/libreoffice/
  cp -R opt/libreoffice*/* "$pkgdir"/usr/lib/libreoffice

}
md5sums=('2d0d1176f72c4b1f1c566f3fe987eef0')
