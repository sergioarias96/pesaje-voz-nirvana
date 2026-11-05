# Pesaje por voz — Granja Nirvana (Exp. 4)

Mobile web app to dictate basket weights by voice and append them to the
Google Sheet *Exp 4. Nirvana - Pesaje manual* (tab `Datos crudos galpones`)
through an Apps Script web app (`AppPesaje.gs`, deployed separately).

- Live app: https://sergioarias96.github.io/pesaje-voz-nirvana/
- The Apps Script `/exec` URL and access token are entered on the phone
  (stored only in that browser). No secrets live in this repository.
- Modes: **Canasta** (basket weights to `Datos crudos galpones`) and **Individual**
  (single-bird weights to `Peso individual galpones`, weekly Friday block
  created automatically by the Apps Script).
- Voice commands: `peso <valor>`, `galpón <n>`, `pollos <n>`, `borrar`; in
  Individual quick mode just the number.
- Requires Chrome on Android with internet for speech recognition; weights
  queue offline and sync when the connection returns.
