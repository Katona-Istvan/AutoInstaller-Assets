# AutoInstaller frissítési fájlok

Ezeket a fájlokat kell az `AutoInstaller-Assets` repó `updates` mappájába feltölteni:

- `latest.json`
- `changelog.txt`
- `README.md`

## Aktuális kiadás

Tag: `v2.61.2`

Telepítő fájl:

`AutoInstallerSetup-v2.61.2.exe`

GitHub Release letöltési link:

`https://github.com/Katona-Istvan/AutoInstaller-Assets/releases/download/v2.61.2/AutoInstallerSetup-v2.61.2.exe`

SHA256:

`1BF0B4841B7A294E8DE4CCA92A971AA5442CEB907AE635ECAB28157B4B84174E`

Fájlméret:

`30901474`

## Fontos sorrend

1. Először készüljön el a GitHub Release `v2.61.2` néven.
2. A release assetek közé kerüljön fel az `AutoInstallerSetup-v2.61.2.exe`.
3. Ezután menjen fel az `updates/latest.json` és `updates/changelog.txt`.

Ha a `latest.json` előbb kerül fel, mint maga a release asset, akkor a régi program már látja az új verziót, de még nem tudja letölteni.
