# DroidStar ADN

Build of [DroidStar](https://github.com/nostar/DroidStar) (GPLv3) for ADN Systems users,
while the upstream pull request [#26](https://github.com/nostar/DroidStar/pull/26) is pending.

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
