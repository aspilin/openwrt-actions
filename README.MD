编译命令如下:

首先装好 Ubuntu 64bit，推荐 Ubuntu 14 LTS x64

sudo apt-get update
sudo apt-get -y install build-essential asciidoc binutils bzip2 gawk gettext git libncurses5-dev libz-dev patch unzip zlib1g-dev lib32gcc1 libc6-dev-i386 subversion flex uglifyjs git-core gcc-multilib p7zip p7zip-full msmtp libssl-dev texinfo libglib2.0-dev xmlto qemu-utils upx libelf-dev autoconf automake libtool autopoint device-tree-compiler

git clone https://github.com/Lienol/openwrt openwrt
或
git clone https://github.com/coolsnowwolf/lede openwrt

./scripts/feeds clean

./scripts/feeds update -a

./scripts/feeds install -a

make menuconfig

[使用 GitHub Actions 云编译 OpenWrt](https://p3terx.com/archives/build-openwrt-with-github-actions.html)
