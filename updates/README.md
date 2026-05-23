# AutoInstaller frissítési csatorna

Ez a mappa az AutoInstaller GitHub alapú önfrissítő rendszeréhez tartozik.

## Fájlok

- `latest.json`: a program ezt olvassa be, hogy megtudja, van-e új verzió.
- `changelog.txt`: emberi nyelvű változáslista, amit a program később meg tud jeleníteni.

## Feltöltés GitHubra

Ezeket a fájlokat a `Katona-Istvan/AutoInstaller-Assets` repóba kell feltölteni ugyanilyen útvonallal:

```text
updates/latest.json
updates/changelog.txt
updates/README.md
```

## Telepítő feltöltése

A telepítőt GitHub Release assetként érdemes feltölteni.

Példa release:

```text
Tag: v2.14.0
Fájl: AutoInstallerSetup-v2.14.0.exe
```

Ha a telepítő fájlneve változik, a `latest.json` fájlban a `downloadUrl` és `fileName` mezőt is frissíteni kell.

## SHA256

A `sha256` mezőbe később a telepítő ellenőrző összege kerül.

PowerShell példa:

```powershell
Get-FileHash .\AutoInstallerSetup-v2.14.0.exe -Algorithm SHA256
```

Az önfrissítő akkor lesz igazán biztonságos, ha letöltés után ellenőrzi, hogy a fájl SHA256 értéke megegyezik-e ezzel.
