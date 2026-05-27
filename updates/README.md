# AutoInstaller frissítési csatorna

Ez a mappa az AutoInstaller GitHub alapú önfrissítő rendszeréhez tartozik.

## Fájlok

- `latest.json`: a program ezt olvassa be, hogy megtudja, van-e új verzió.
- `changelog.txt`: emberi nyelvű változáslista, amit a program később meg tud jeleníteni.
- `README.md`: rövid leírás a frissítési csatorna használatához.

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
Tag: v2.18.1
Fájl: AutoInstallerSetup-v2.18.1.exe
```

Ha a telepítő fájlneve változik, a `latest.json` fájlban a `downloadUrl` és `fileName` mezőt is frissíteni kell. A `Installer/Build-Release.ps1` script ezt helyben automatikusan frissíti.

## SHA256

A `sha256` mezőbe a telepítő ellenőrző összege kerül. Ez azért kell, hogy az önfrissítő később ellenőrizni tudja: pontosan azt a telepítőt töltötte-e le, amit kiadtál.

PowerShell példa:

```powershell
Get-FileHash .\AutoInstallerSetup-v2.18.1.exe -Algorithm SHA256
```
