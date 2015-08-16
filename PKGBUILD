# Contributor: atie H. <atie.at.matrix_at_gmail_dot_com>
# Editer: ujuc <ujuc_at_ujuc_dot_kr>
# Thank to: zinc <aeiou256_at_naver_dot_com>, bsjeon <bsjeon_at_hanmail_dot_net>

pkgname=nabi
pkgver=1.0.0
pkgrel=4
pkgdesc="Easy and Powerful GNU XIM for Korean in X Window System"
arch=(i686 x86_64)
url="http://code.google.com/p/nabi/"
license=('GNU GPL v2')
depends=('gtk2' 'libhangul>=0.1.0')
source=(https://nabi.googlecode.com/files/nabi-1.0.0.tar.gz)
md5sums=('15d0adbb92698ccd7171b4a5c7991d12')

build() {
    cd "$startdir/src/$pkgname-$pkgver"

    ./configure --prefix=/usr
    make
}

package() {
    cd "$srcdir/$pkgname-$pkgver"

    make DESTDIR="$pkgdir" install
}
