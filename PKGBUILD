# Maintainer: @zstg <zestig@duck.com>
pkgname=stratos-hyprland-config
pkgver=1.0
pkgrel=1
pkgdesc="Hyprland configuration for StratOS"
arch=('any')
license=('GPL3')
depends=(
    'hyprland' 'hyprpaper' 'hypridle' 'hyprlock'
    'waybar' 'stratos-waybar-config'
    'kitty' 'stratos-kitty-config'
    'stratos-eww-config'
    'mako' 'stratos-mako-config'
)
optdepends=( 
    'stratos-btop-config: system resource monitor'
    'stratmacs: app launchers'
    'rofi: alternate app launcher'
)
source=('.config')
md5sums=('SKIP')

package() {
    install -d "$pkgdir/etc/skel/.config"
    cp -r "$srcdir/.config/hypr/" "$pkgdir/etc/skel/.config/"
    echo "Configuration files have been copied to /etc/skel."
    echo "You may copy these files to ~/.config/ and make any changes you wish."
}
