# Maintainer: shiliang <shiliang2008@msn.com>

pkgname=chez-srfi
_pkgname=chez-srfi
pkgdesc='SRFI for ChezScheme'
pkgver=1.1
pkgrel=1
arch=('any')
url='https://github.com/shih-liang/chez-srfi.git'
license=('MIT')
depends=('chez-scheme')

source=( ${_pkgname}-${pkgver}-${pkgrel}-${_arch}.tar.gz::https://github.com/fedeinthemix/chez-srfi/archive/refs/tags/v1.0.tar.gz)
md5sums=('SKIP')
provides=('chez-srfi')

build(){
  cd chez-srfi-1.0
  make CHEZ=scheme
}
package(){
  cd chez-srfi-1.0
  make install CHEZ=scheme PREFIX=${pkgdir}/usr
}
