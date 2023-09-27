# Generell

## Hochschulinternes WLAN

### HsKA-8021x

```
Security:             WPA/WPA2 Enterprise
Authentication:       Tunneled TLS
[x] No CA certificate is required
Inner authentication: MSCHAPv2 (no EAP)
Username:             <RZ Kürzel>@<Fakultät Kürzel>-wlan.h-ka.de
Password:             <RZ Password>
```

### VPN

* AnyConnect:
  * Alternative: `sudo apt install network-manager-vpnc-gnome`
  * Offiziel (nicht getestet): <https://www.cisco.com/c/de_de/support/docs/smb/routers/cisco-rv-series-small-business-routers/Kmgmt-785-AnyConnect-Linux-Ubuntu.html>

## [eduroam](https://eduroam.org/)

Von der Webseite [rz.h-ka.de/eduroam](https://rz.h-ka.de/eduroam) das installer Skript herunterladen und dann ausführen.

## [bwSync&Share](https://bwsyncandshare.kit.edu)
[bwSync&Share Client](https://customerupdates.nextcloud.com/kk1eoZCTo0kI5HpGE3IT/)

## PDF Mitschreiben

* [Xournal++](https://xournalpp.github.io/)
  * <https://xournalpp.github.io/installation/linux/>
  * `sudo apt install xournalpp`

* [Rnote](https://rnote.flxzt.net/)
  * [Flatpak](https://flathub.org/apps/com.github.flxzt.rnote)
  
## Office Documente

* [LibreOffice](https://de.libreoffice.org/): nahezu immer vorinstalliert
  
## $\LaTeX$

* [TexLive](https://www.tug.org/texlive/quickinstall.html)
* Eiditor:
  * [TeXstudio](https://www.texstudio.org/)
  * [Texmaker](https://www.xm1math.net/texmaker/)
  * [VSCode Extention](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop)

## Chatprogramme

### [Signal](https://signal.org/de/)

* <https://signal.org/download/linux/>

```bash
# NOTE: These instructions only work for 64 bit Debian-based
# Linux distributions such as Ubuntu, Mint etc.

# 1. Install our official public software signing key
wget -O- https://updates.signal.org/desktop/apt/keys.asc | gpg --dearmor > signal-desktop-keyring.gpg
cat signal-desktop-keyring.gpg | sudo tee -a /usr/share/keyrings/signal-desktop-keyring.gpg > /dev/null

# 2. Add our repository to your list of repositories
echo 'deb [arch=amd64 signed-by=/usr/share/keyrings/signal-desktop-keyring.gpg] https://updates.signal.org/desktop/apt xenial main' |\
  sudo tee -a /etc/apt/sources.list.d/signal-xenial.list

# 3. Update your package database and install signal
sudo apt update && sudo apt install signal-desktop
```
```bash
# NOTE: These instuctions are for flatpak

# 1. Add Flathub to Flatpak
flatpak remote-add --if-not-exists flathub https://dl.flathub.org/repo/flathub.flatpakrepo

# 2. Install Signal
flatpak install flathub org.signal.Signal
```

### [Discord](https://discord.com/)
Für Debian Basierte Systeme:
1. Downloade das `.deb` Packet von <https://discord.com/download>.
2. Installieren:
   * **Visuel**: Doppelklick auf das Deb Packet und auf installieren klicken.
   * **Terminal**: im Terminal `sudo apt install "<vollstaendigerPfad>/discord.deb"`

Alternativ mit [Flatpak](https://flatpak.org/):
```bash
# NOTE: These instuctions are for flatpak

# 1. Add Flathub to Flatpak
flatpak remote-add --if-not-exists flathub https://dl.flathub.org/repo/flathub.flatpakrepo

# 2. Install Discord
flatpak install flathub com.discordapp.Discord
```
