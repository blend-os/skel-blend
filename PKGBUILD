pkgname=skel-blend
pkgver=2023.01.01
pkgrel=1
pkgdesc='Skel configuration for blendOS'
url='https://github.com/blend-os/skel-blend'
arch=('any')
conflicts=('grml-zsh-config')
license=('Public domain')
source=('init.vim' '.zshrc' '.zprofile')
sha256sums=('6f9f17c50e8566fb18960beb05d155b4439b9b42269dd9720f001e91aa50bc8f'
            '75a02d8721f6a8eb2324a34609eb556e0120ad86a2a1bf86a595651231ec8730'
            '1fc8a69b750aa7870eb31a0d9ae4f47ffb4c0bbd59adc1a17984295405f8d27a')

package() {
	cd "$pkgdir"

	install -d etc/skel/.config/nvim

	install -m644 "$srcdir"/init.vim etc/skel/.config/nvim/
	install -m644 "$srcdir"/.zshrc etc/skel/
}

