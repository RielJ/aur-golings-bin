# Maintainer: Riel Joseph <bulaybulay.rielj@gmail.com>
#
pkgname=golings-bin
pkgver=0.6.2
pkgrel=1
pkgdesc="Rustlings for Golang this time"
arch=('x86_64')
url="https://github.com/mauricioabreu/golings"
license=('APACHE')
depends=('go')
provides=("golings")
conflicts=("golings")
install="golings.install"
source_x86_64=("golings_${pkgver}_Linux_x86_64.tar.gz::https://github.com/mauricioabreu/golings/releases/download/v${pkgver}/golings_${pkgver}_Linux_x86_64.tar.gz")
sha256sums_x86_64=('3235016060403a807961d5bda9643104fea022a6283eb09ebb4bbc36131a28c7') 

package() {
  install -D golings -t "$pkgdir"/usr/bin/
  install -Dm 644 README.md -t "$pkgdir"/usr/share/doc/$pkgname
  install -Dm 644 LICENSE -t "$pkgdir"/usr/share/licenses/$pkgname
}
