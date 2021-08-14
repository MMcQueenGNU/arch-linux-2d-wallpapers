# Maintainer: McQueen <clear3239@yahoo.com>
_pkgname=arch-linux-2d
pkgname=arch-linux-2d-wallpapers
pkgver=1.0.1
pkgrel=1
pkgdesc='Collection of Arch Logo 2D Wallpapers'
arch=(any)
url='https://wallpaperzone.tumblr.com/tagged/linux/page/3'
_url="https://github.com/MMcQueenGNU"
license=('CC-BY-SA')
source=("$_url/$pkgname/archive/refs/tags/v$pkgver.tar.gz")

md5sums=('23be1bf75a8836a297bb367e83aa552c')

package() {

	cd "$srcdir/$pkgname-$pkgver/$_pkgname"

	# Creating needed directories
	install -dm755 "${pkgdir}/usr/share/backgrounds/$_pkgname/"

	# Wallpapers
	local wallpaper
	for wallpaper in *; do
		install -m755 "$srcdir/$pkgname-$pkgver/$_pkgname/${wallpaper}" "$pkgdir/usr/share/backgrounds/$_pkgname/${wallpaper}"
	done
}
