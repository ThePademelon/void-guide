You'll need to generate WireGuard config files withe Mullvad's [config file generator](https://mullvad.net/en/account/#/wireguard-config/).

Install WireGuard and unzip
```bash
sudo xbps-install wireguard
sudo xbps-install unzip
```

Unzip .conf files and send them to wireguard
```bash
cd ~/Downloads
unzip mullvad_wireguard_linux_*.zip
sudo mv *.conf /etc/wireguard
```

I used Switzerland's ch2 server so my location alias is ch2, **yours will be different** if you didn't select Switzerland's ch2 server.

Turn on VPN (ch2)
```bash
wg-quick up mullvad-ch2
```

Turn off VPN (ch2)
```bash
wg-quick down mullvad-ch2
```
