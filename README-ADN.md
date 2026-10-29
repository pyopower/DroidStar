# DroidStar ADN

Build of [DroidStar](https://github.com/nostar/DroidStar) (GPLv3) for ADN Systems users,
while the upstream pull request [#26](https://github.com/nostar/DroidStar/pull/26) is pending.

> **Unofficial build.** DroidStar is written by Doug McLain (nostar) and contributors; this is a
> modified version made for the ADN Systems community. Please report problems with it here,
> not to the DroidStar author.
>
> **Versión no oficial.** DroidStar es obra de Doug McLain (nostar) y colaboradores; esta es una
> versión modificada para la comunidad de ADN Systems. Los problemas con ella, aquí, no al autor de DroidStar.

## License / Licencia

GNU GPL v3 or later, like DroidStar (see the file headers). Full text in [COPYING](COPYING).
The source of every release is its `adn-*` tag on the `adn-systems` branch.

GNU GPL v3 o posterior, como DroidStar. Texto completo en [COPYING](COPYING). El código de cada
versión es su tag `adn-*` de la rama `adn-systems`.

## What it changes

- **ADN Pass** in Settings (under TGIF Pass): your ADN Systems selfcare password.
  It is used for the `FD_ADN_*` / `ADN*` hosts, like the BM and TGIF passwords.
  Without it, ADN servers that require an individual password reject the login.
- Own package id (`ovh.adan.droidstar`) and name (**DroidStar ADN**), so it installs
  next to the official DroidStar without replacing it.
- Built with the internal software vocoder (no md380 library).

Branch `adn-systems` = upstream `main` + PR #26 + the build changes above.

---

## Qué cambia (ES)

- **ADN Pass** en Ajustes (debajo de TGIF Pass): tu contraseña de selfcare de ADN Systems.
  Se usa en los servidores `FD_ADN_*` / `ADN*`, igual que las de BM y TGIF.
  Sin ella, los servidores ADN que piden contraseña individual rechazan la conexión.
- Paquete (`ovh.adan.droidstar`) y nombre (**DroidStar ADN**) propios: se instala junto
  al DroidStar oficial sin sustituirlo.
- Compilado con el vocoder por software interno (sin la librería md380).

## Builds / Compilación

GitHub Actions (`.github/workflows/adn-android.yml`) builds and signs the APK.
Push a tag `adn-<version>-<versionCode>` (e.g. `adn-1.0-97`; the code must go up) and the
APK is attached to that release. *Run workflow* by hand leaves it as a build artifact.
Signing key: repository secrets `ADN_KEYSTORE_B64` and `ADN_KEYSTORE_PASSWORD`.

Para sacar una versión nueva: tag `adn-<versión>-<versionCode>` (el versionCode siempre mayor);
la APK firmada aparece en la release de ese tag.
