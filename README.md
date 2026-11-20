# RIN by OSRIN

Clickable design mockup of RIN: the owner dashboard (cube-shaped Campus map + rin chat), with log in, sign up, request sent and signed out as separate pages. Light theme only.

Every screen is its own HTML file. Nothing is built or bundled, and there are no dependencies. Open any file in a browser.

## Files

- `index.html`: the main dashboard. Map, rin chat, approvals, profile menu. Not embedded in or tied to the login pages.
- `parts/approval.html`: the approval card in the rin chat. Embedded in the dashboard; talks to it with `postMessage` (the page sends the approval, the card sends back the option picked). Open it alone to see a sample card.
- `parts/connections.html`: the connected apps (MCPs or tools) around the map. Each app is a dot with a line to each department that uses it. An app two departments share is one dot. Gatehouse and Governance have none. Edit `CONNECTIONS` at the top of the file.
- `departments/*.html`: one page per department (plus `rin.html`), sharing `department.css`. Open them from the map ("Open <department> →"); "Back to map" returns to `index.html`.
- `auth/login.html`, `auth/signup.html`, `auth/request-sent.html`, `auth/signed-out.html`: the account pages, each standalone. They link to each other and Log in links to `../index.html`.
- `logo-animation/`: the logo animation files.

The only link from the dashboard to the account pages is "Exit" in the profile menu, which opens `auth/signed-out.html`.

All data is sample data. Nothing is sent, saved or paid. Screen names are placeholders until confirmed.
