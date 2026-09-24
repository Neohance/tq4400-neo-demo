# TQ 4400 NeO — interactive demo

Interactive 3D model and HMI demonstration of the Neohance TQ 4400 NeO electronics upgrade for the TQ 4400 TankScan gas sampling system.

- `index.html` is the complete demo in one file (3D model, touchscreen simulation, guided tour, EN/NL).
- Published with GitHub Pages: Settings → Pages → Source: *Deploy from a branch* → `main` / `(root)`.
- The page carries `noindex` so search engines are asked not to list it; anyone with the link can still open it.

Demonstration model: timings are shortened and the cabinet interior is indicative. Operation as described in the TQ 4400 NeO manual.

Neohance B.V. · Olivijn 522, 3316 KH Dordrecht · neohance.tech

Third-party: three.js r149 (MIT licence, © 2010–2023 three.js authors), embedded in `index.html`.

## Microsoft Teams

`teams/tq4400-neo-demo-teams.zip` is a Teams app package (manifest v1.17 + icons) that opens the demo as a personal tab.

- Upload: Teams → Apps → Manage your apps → *Upload an app* → *Upload a custom app* (needs custom-app upload allowed in the Teams admin center), or an admin publishes it for the organisation via Teams admin center → Manage apps → Upload new app.
- GitHub Pages sends no `X-Frame-Options` or `frame-ancestors` header, so Teams may frame the page; it is served over HTTPS.
- Inside a frame the page loads `vendor/MicrosoftTeams.min.js` (TeamsJS 2.57.0, MIT, © Microsoft) and reports itself loaded to Teams. Opened directly, nothing extra loads.
- After changing `teams/manifest.json` or the icons, raise `version` and rebuild: `cd teams && zip -X tq4400-neo-demo-teams.zip manifest.json color.png outline.png`.
