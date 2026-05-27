# AutoInstaller frissítési fájlok

Ezeket a fájlokat kell az `AutoInstaller-Assets` repó `updates` mappájába feltölteni:

- `latest.json`
- `changelog.txt`
- `README.md`

## Aktuális kiadás

Tag: `v2.19.0`

Telepítő fájl:

`AutoInstallerSetup-v2.19.0.exe`

GitHub Release letöltési link:

`https://github.com/Katona-Istvan/AutoInstaller-Assets/releases/download/v2.19.0/AutoInstallerSetup-v2.19.0.exe`

SHA256:

`B1376F9D145BFB27BB041D56A09BA2D9DD0A637FFAAABFFEE18D6879E52CBB3D`

Fájlméret:

`30112281`

## Fontos sorrend

1. Először készüljön el a GitHub Release `v2.19.0` néven.
2. A release assetek közé kerüljön fel az `AutoInstallerSetup-v2.19.0.exe`.
3. Ezután menjen fel az `updates/latest.json` és `updates/changelog.txt`.

Ha a `latest.json` előbb kerül fel, mint maga a release asset, akkor a régi program már látja az új verziót, de még nem tudja letölteni.
