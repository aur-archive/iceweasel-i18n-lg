# Contributor: jorge_barroso <jorge.barroso.11@gmail.com>"
# Contributor: mar77i <mysatyre at gmail dot com>"

_debname=iceweasel
_debver=16.0.1
_debrel=1
_debrepo=http://ftp.debian.org/debian/pool/main/

pkgname=iceweasel-i18n-lg
pkgver=$_debver
pkgrel=1
groups=('iceweasel-i18n')
pkgdesc="Language packs for Debian Iceweasel."
arch=('any')
url="http://www.geticeweasel.org/"
license=('MPL')
depends=("iceweasel>=$_debver")

source=("$_debrepo/${_debname:0:1}/$_debname/$_debname-l10n-lg_${_debver}-${_debrel}_all.deb")
md5sums=(8dbd143d46cc51b373f6b61f1a27d6f4)

build() {
	cd "$srcdir"
	bsdtar xf "${source##*/}"
	cd "$pkgdir"
	tar Jxf "$srcdir"/data.tar.xz
}


