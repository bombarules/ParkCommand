# PoolCommand

Aquatics operations board for the park's seven pools: Splash Landing, Aviator, F-15, Jet Stream, Puddle Jumper, Maverick and Runway 35.

- **Board**: every pool as a flight strip showing status, latest free chlorine and pH, and when it was last tested. Out-of-range values turn red; open pools past their test interval are marked Due.
- **Weather hold**: one tap clears every open pool and starts a 30-minute clock. "Strike again" resets it; "End hold" reopens the pools that were open.
- **Pool panel**: set Open / Closed / Maintenance, log readings (free and combined chlorine, pH, temperature), see trends, and record parts replaced.
- **Log**: one timeline of readings, parts, incidents, rescues, first aid and notes, with initials.
- **Checks**: daily opening checklist per pool, editable, resets each morning.
- **More**: ranges to match your local health code, CSV export of readings, full backup and restore.

Everything works offline and is stored on the phone.

## Build
Push to `main` (or run the workflow from the Actions tab). The APK appears on the Releases page under **latest**.

The app is a WebView shell (`PoolCommand/app/src/main/java/.../MainActivity.kt`) around `PoolCommand/app/src/main/assets/index.html`. To change the app, edit that HTML file and bump `versionCode` / `versionName` in `PoolCommand/app/build.gradle.kts`.
