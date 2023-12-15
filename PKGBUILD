#Contributor: abcd567
# Maintainer: abcd567

pkgname=rbfeeder
pkgver=1.0.10+bullseye
pkgrel=0
pkgdesc="ADS-B Data Feeder of RadarBox24.com"
url="https://www.radarbox.com/sharing-data"
license=('GPL')

makedepends=('fakeroot')
depends=('protobuf-c' 'jansson' 'rtl-sdr')

arch=('armv6h' 'armv7h' 'arm64' 'aarch64')
source_armv6h=("https://apt.rb24.com/pool/main/r/rbfeeder/rbfeeder_${pkgver}_armhf.deb")
source_armv7h=("https://apt.rb24.com/pool/main/r/rbfeeder/rbfeeder_${pkgver}_armhf.deb")
source_aarch64=("https://apt.rb24.com/pool/main/r/rbfeeder/rbfeeder_${pkgver}_arm64.deb")

sha256sums_armv6h=('SKIP')
sha256sums_armv7h=('SKIP')
sha256sums_aarch64=('SKIP')

install=rbfeeder.install

backup=(etc/rbfeeder.ini)


package() {
  bsdtar -xf data.tar.xz -C "$pkgdir/"
  mv "$pkgdir/lib" "$pkgdir/usr/"
}

