# Maintainer: Greg Fitzgerald <greg@gregf.org>
pkgname=parbench
pkgver=1.3.2
pkgrel=3
pkgdesc="Visual HTTP Concurrency / Load Tool"
arch=('i686' 'x86_64')
url="https://github.com/andrewvc/engulf"
license=('MIT')
depends=(java-runtime)
source=("https://github.com/downloads/andrewvc/engulf/${pkgname}-${pkgver}-standalone.jar"
        ${pkgname}.sh)
md5sums=('afb1ce8f8211528e81b63cb68eb3a15b'
         '027c0e5a937d9d63a896983473e309c9')
noextract=(${source[@]##*/})

package() {
  cd "${srcdir}"
  install -Dm755 ${pkgname}.sh "${pkgdir}"/usr/bin/${pkgname}
  install -Dm644 ${pkgname}-${pkgver}-standalone.jar "${pkgdir}"/usr/share/java/parbench/${pkgname}.jar
}

# vim:set ts=4 sw=4 et:
