openwrt
=
Version:19.07.7

update logs : https://openwrt.org/releases/19.07/changelog-19.07.7

Compilation steps:

1 sudo apt-get -y install build-essential asciidoc binutils bzip2 gawk gettext git libncurses5-dev libz-dev patch python3 python2.7 unzip zlib1g-dev lib32gcc1 libc6-dev-i386 subversion flex uglifyjs git-core gcc-multilib p7zip p7zip-full msmtp libssl-dev texinfo libglib2.0-dev xmlto qemu-utils upx libelf-dev autoconf automake libtool autopoint device-tree-compiler g++-multilib antlr3 gperf wget curl swig rsync

2 mkdir openwrt

3 sudo chmod 777 openwrt

4 cd openwrt

5 git clone https://github.com/Tonkercke/openwrt.git

6 cd openwrt

7 ./scripts/feeds update -a

8 ./scripts/feeds install -a

9 make menuconfig

10 make V=99

