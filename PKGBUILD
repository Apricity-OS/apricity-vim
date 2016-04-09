#Maintainer: Alex Gajewski <agajews@gmail.com>

_pkgname='Apricity Vim'
pkgname=apricity-vim
pkgver=0.1.1
pkgrel=1
pkgdesc='Vim config for Apricity OS'
arch=(any)
license=(GPL)
url="https://github.com/ApricityOS"
source=("apricity-vim.tar.gz")
sha256sums=(SKIP)

package() {
	mkdir -p "${pkgdir}/etc/skel/"
	cp -rf "${srcdir}/apricity-vim/.vim" "${pkgdir}/etc/skel"
	cp -f "${srcdir}/apricity-vim/.vimrc" "${pkgdir}/etc/skel"

	mkdir -p "${pkgdir}/root/"
	cp -rf "${srcdir}/apricity-vim/.vim" "${pkgdir}/root"
	cp -f "${srcdir}/apricity-vim/.vimrc" "${pkgdir}/root"
}
