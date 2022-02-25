Install flatpak
```bash
sudo xbps-install -S flatpak
flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
```

Install Mailspring
```bash
flatpak install flathub com.getmailspring.Mailspring
```

Run Mailspring
```bash
flatpak run com.getmailspring.Mailspring
```