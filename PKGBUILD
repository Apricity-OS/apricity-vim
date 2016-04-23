#Maintainer: Alex Gajewski <agajews@gmail.com>

_pkgname='Apricity Vim'
pkgname=apricity-vim
pkgver=0.1.3
pkgrel=1
pkgdesc='Vim config for Apricity OS'
arch=(any)
license=(GPL)
install="apricity-vim.install"
url="https://github.com/ApricityOS"
source=("apricity-vim.tar.gz")
sha256sums=(SKIP)

package() {
	mkdir -p "${pkgdir}/etc/skel/"
	rm -rf "${pkgdir}/etc/skel/.vim"
	rm -f "${pkgdir}/etc/skel/.vimrc"
	cp -rf "${srcdir}/apricity-vim/.vim" "${pkgdir}/etc/skel"
	cp -f "${srcdir}/apricity-vim/.vimrc" "${pkgdir}/etc/skel"

	mkdir -p "${pkgdir}/root/"
	rm -rf "${pkgdir}/root/.vim"
	rm -f "${pkgdir}/root/.vimrc"
	cp -rf "${srcdir}/apricity-vim/.vim" "${pkgdir}/root"
	cp -f "${srcdir}/apricity-vim/.vimrc" "${pkgdir}/root"
}
