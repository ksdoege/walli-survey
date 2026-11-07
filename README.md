# Walli Survey — offline edition

Home-screen web app version of the Walli stylist/barber field survey. Caches itself on the iPad (service worker), saves every response on-device, and POSTs queued rows to the Apps Script backend (`doPost`, token-guarded) whenever there is signal. Same Google Sheet, same tabs, same columns as the Apps Script web app.

- Live: https://ksdoege.github.io/walli-survey/
- Source of truth for questions: this `index.html` and the Apps Script project's `Index.html` are kept in step by hand — change both.
- After editing `index.html`, bump `CACHE` in `sw.js` so installed iPads pick up the new build.
