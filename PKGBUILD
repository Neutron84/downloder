# Maintainer: Doug Newgard <scimmia at archlinux dot info>

pkgname=pepper-flash
pkgver=32.0.0.465
pkgrel=1
pkgdesc="Adobe's Pepper Flash plugin"
arch=('i686' 'x86_64')
url='https://get.adobe.com/flashplayer/'
license=('custom')
depends=('gcc-libs' 'glibc')
optdepends=('flashplugin: Settings utility')
conflicts=('chromium-pepper-flash')
source_i686=("flash_player_ppapi_linux_${pkgver}.i386.tar.gz::https://fpdownload.adobe.com/get/flashplayer/pdc/${pkgver}/flash_player_ppapi_linux.i386.tar.gz")
source_x86_64=("flash_player_ppapi_linux_${pkgver}.x86_64.tar.gz::https://fpdownload.adobe.com/get/flashplayer/pdc/${pkgver}/flash_player_ppapi_linux.x86_64.tar.gz")
sha256sums_i686=('daa8d7f3bc1e8d9af651ecd59958da7c955fb20f8602b5b524570f9315db233d')
sha256sums_x86_64=('2fac28d1d7723fec39709f9db2b606d8ceba410f153c34f76397d23ac0d62bce')

package() {
  install -Dm644 manifest.json libpepflashplayer.so -t "$pkgdir/usr/lib/PepperFlash/"
  install -Dm644 license.pdf -t "$pkgdir/usr/share/licenses/$pkgname/"
}