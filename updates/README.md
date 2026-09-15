# AutoInstaller frissítési fájlok

Ezeket a fájlokat kell az `AutoInstaller-Assets` repó `updates` mappájába feltölteni:

- `latest.json`
- `changelog.txt`
- `README.md`

## Aktuális kiadás

Tag: `v2.61.1`

Telepítő fájl:

`AutoInstallerSetup-v2.61.1.exe`

GitHub Release letöltési link:

`https://github.com/Katona-Istvan/AutoInstaller-Assets/releases/download/v2.61.1/AutoInstallerSetup-v2.61.1.exe`

SHA256:

`F48CBBA3336F4973347CC2C109E3E92F9204E6CED657CD9395B35347067BC5E3`

Fájlméret:

`30897407`

## Fontos sorrend

1. Először készüljön el a GitHub Release `v2.61.1` néven.
2. A release assetek közé kerüljön fel az `AutoInstallerSetup-v2.61.1.exe`.
3. Ezután menjen fel az `updates/latest.json` és `updates/changelog.txt`.

Ha a `latest.json` előbb kerül fel, mint maga a release asset, akkor a régi program már látja az új verziót, de még nem tudja letölteni.
