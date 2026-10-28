# RoDesk Remote

Client de asistență la distanță al Teron Systems SRL, construit din [RustDesk](https://github.com/rustdesk/rustdesk) 1.5.0
(licență AGPL-3.0, © Purslane Tech Pte. Ltd.). Sursa completă a versiunii distribuite este acest depozit, ramura `rodesk-remote`.

## Ce diferă față de RustDesk 1.5.0
- `libs/hbb_common` (prin `rodesk/hbb_common.patch`, aplicat la compilare): numele aplicației `RoDeskRemote`,
  serverul `remote.teron.ro` și cheia lui publică, opțiunea fixă `hide-powered-by-me`, afișarea implicită „adaptive” (ecranul la distanță se potrivește la fereastră).
- `src/lang.rs`: în texte, numele afișat este „RoDesk Remote” (numele intern rămâne fără spațiu, pentru serviciul Windows).
- `flutter/windows/runner/Runner.rc`, `Cargo.toml`, `libs/portable/Cargo.toml`: datele fișierului (produs, firmă, descriere).
- Iconițele din `res/`, `flutter/windows/runner/resources/` și `flutter/assets/`.
- Linkul „Declarație de confidențialitate” trimite la https://remote.teron.ro/.
- `.github/workflows/rodesk-remote.yml`: compilarea Windows x64 și împachetarea în `RoDeskRemote.exe`.

Mențiunile de licență și drepturile de autor RustDesk din „Despre” sunt păstrate.
