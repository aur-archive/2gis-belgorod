pkgname=2gis-belgorod
pkgver=24
pkgrel=1
pkgdesc="Map of Belgorod for 2GIS, June 2013"
arch=('i686' 'x86_64')
url="http://belgorod.2gis.ru/how-get/linux/"
license=('custom')
depends=('2gis>=3.13.5.1')
source=("http://download.2gis.ru/arhives/2GISData_Belgorod-24.orig.zip")
md5sums=('5ef8303220dde190f23fe2d76a361b27')

package() {
  install -D -m 644 "${srcdir}/2gis/3.0/Data_Belgorod.dgdat" "${pkgdir}/opt/2gis/belgorod.dgdat" || return 1
  install -D -m 644 "${srcdir}/2gis/3.0/Plugins/DGisLan/Belgorod.dglf" "${pkgdir}/opt/2gis/Plugins/DGisLan/belgorod.dglf" || return 1
}
