Clone and enter the void-packages repository
```bash
git clone https://github.com/void-linux/void-packages.git
cd void-packages
```

Setup xbps-src and allow [restricted packages](https://docs.voidlinux.org/xbps/repositories/restricted.html#restricted-packages)
```bash
./xbps-src binary-bootstrap
echo XBPS_ALLOW_RESTRICTED=yes >> etc/conf
```

Build and install Discord
```bash
./xbps-src pkg discord
sudo xbps-install --repository hostdir/binpkgs/nonfree discord
```

Run Discord
```bash
Discord
```
