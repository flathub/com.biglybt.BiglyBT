# com.biglybt.BiglyBT
Flatpak for BiglyBT (https://www.biglybt.com/)

## Prerequisite

- `flatpak`, `flatpak-builder` packages
- Runtime `org.freedesktop.Platform` version `22.08`
- Runtime `org.freedesktop.Sdk` version `22.08`
- Runtime Extension `org.freedesktop.Sdk.Extension.openjdk`

## Method 1:

### Build and install BiglyBT
```bash
flatpak-builder --user --install --force-clean  flatpakbuildir com.biglybt.BiglyBT.yaml
```
### Run BiglyBT
```bash
flatpak run com.biglybt.BiglyBT
```
### Uninstall BiglyBT
```bash
flatpak uninstall --user com.biglybt.BiglyBT
```


## Method 2:

### Build BiglyBT
```bash
flatpak-builder --repo=repo --force-clean flatpakbuildir com.biglybt.BiglyBT.yaml
```
### Add BiglyBT local repo
```bash
flatpak remote-add --user mybiglybt repo
```
### Install BiglyBT from local repo
```bash
flatpak install --user mybiglybt com.biglybt.BiglyBT
```
### Run BiglyBT
```bash
flatpak run com.biglybt.BiglyBT
```
### Uninstall BiglyBT
```bash
flatpak uninstall --user com.biglybt.BiglyBT
```
