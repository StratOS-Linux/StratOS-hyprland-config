# Maintainer: @magitian <magitian@duck.com>
pkgname=stratos-hyprland-config
pkgver=1.0
pkgrel=3
pkgdesc="Hyprland configuration for StratOS"
arch=('any')
license=('GPL3')
depends=(
    'hyprland' 'hyprpaper' 'hypridle' 'hyprlock'
    'waybar' 'stratos-waybar-config'
    'kitty' 'stratos-kitty-config'
    'eww' 'stratos-eww-config'
    'stratos-fonts'
    'mako' 'stratos-mako-config'
    'swayosd-git'
    'polkit-gnome'
    'nwg-dock-hyprland-bin'
)

optdepends=(
    'stratmacs: StratOS Emacs build'
    'stratmacs-config: Stratmacs configuration'
    'stratos-btop-config: system resource monitor'
    'swaync: recommended notification daemon'
    'stratos-wallpapers: default wallpapers provided by the StratOS team'
    'libqalculate: command-line scientific calculator, needed for calc script'
    'rofi: alternate app launcher'
)

source=()
md5sums=('SKIP')
install=stratos-hyprland-config.install

package() {
    install -d "$pkgdir/etc/skel/.config"
    cp -r "$srcdir/.config/hypr/" "$pkgdir/etc/skel/.config/"
}
