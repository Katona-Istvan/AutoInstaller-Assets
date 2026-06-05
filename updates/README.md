# AutoInstaller frissítési fájlok

Ezeket a fájlokat kell az `AutoInstaller-Assets` repó `updates` mappájába feltölteni:

- `latest.json`
- `changelog.txt`
- `README.md`

## Aktuális kiadás

Tag: `v2.19.1`

Telepítő fájl:

`AutoInstallerSetup-v2.19.1.exe`

GitHub Release letöltési link:

`https://github.com/Katona-Istvan/AutoInstaller-Assets/releases/download/v2.19.1/AutoInstallerSetup-v2.19.1.exe`

SHA256:

`F935F3D697A9B43E116C131458C9536A708E14528BF4CBABDBEC730B367894B3`

Fájlméret:

`30116358`

## Fontos sorrend

1. Először készüljön el a GitHub Release `v2.19.1` néven.
2. A release assetek közé kerüljön fel az `AutoInstallerSetup-v2.19.1.exe`.
3. Ezután menjen fel az `updates/latest.json` és `updates/changelog.txt`.

Ha a `latest.json` előbb kerül fel, mint maga a release asset, akkor a régi program már látja az új verziót, de még nem tudja letölteni.
