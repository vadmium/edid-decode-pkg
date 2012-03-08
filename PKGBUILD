pkgname=edid-decode
_commit=95019a3
_ver=77
pkgver="${_ver}_g${_commit}"
_snapshot="$pkgname-$_ver-g$_commit"
pkgrel=1
pkgdesc="EDID decoder and conformance tester"
url="http://cgit.freedesktop.org/xorg/app/$pkgname"
arch=('i686' 'x86_64')
license=('MIT')
source=("$url/snapshot/$_snapshot.tar.gz")
md5sums=(4cf04ffbca1dc8f0cc96330a361e488c)

build() {
    make -C "$srcdir/$_snapshot"
}

package() {
    make -C "$srcdir/$_snapshot" install DESTDIR="$pkgdir"
}
