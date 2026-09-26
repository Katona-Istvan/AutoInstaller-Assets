# AutoInstaller frissítési fájlok

Ezeket a fájlokat kell az `AutoInstaller-Assets` repó `updates` mappájába feltölteni:

- `latest.json`
- `changelog.txt`
- `README.md`

## Aktuális kiadás

Tag: `v2.61.3`

Telepítő fájl:

`AutoInstallerSetup-v2.61.3.exe`

GitHub Release letöltési link:

`https://github.com/Katona-Istvan/AutoInstaller-Assets/releases/download/v2.61.3/AutoInstallerSetup-v2.61.3.exe`

SHA256:

`3D3C73B3CA568D2C798F931834CA22C2C349BF6C65F58E5C9C7BEE138FC86537`

Fájlméret:

`30911593`

## Fontos sorrend

1. Először készüljön el a GitHub Release `v2.61.3` néven.
2. A release assetek közé kerüljön fel az `AutoInstallerSetup-v2.61.3.exe`.
3. Ezután menjen fel az `updates/latest.json` és `updates/changelog.txt`.

Ha a `latest.json` előbb kerül fel, mint maga a release asset, akkor a régi program már látja az új verziót, de még nem tudja letölteni.
