# RIN by OSRIN

Clickable design mockup of RIN, using the MJ map with the cube-shaped land (17 Nov): log in, sign up (lead form), request sent, the owner dashboard with the Campus map and the profile menu, and the signed-out screen.

This cut is light theme only and Campus map only. The theme switch, dark tones and map style switch are removed.

## Files

- `index.html`: log in, sign up, request sent, the Campus map dashboard with the profile menu, and signed out.
- `departments/`: one page per department (`accounting.html`, `market.html`, `gatehouse.html`, `care.html`, `marketing.html`, `library.html`, `workshop.html`, `governance.html`, and `rin.html` for RIN itself). They all share `department.css`. Each page summarises what the department has (helpers, rules, connected apps) and what it did today.

On the map, click a department, then **Open <department> →** to go to its page. **Back to map** returns to the dashboard.

## Run

Open `index.html` in a browser. There is no build step and there are no dependencies. Keep the `departments/` folder next to `index.html`.

All data is sample data. Nothing is sent, saved or paid. Screen names are placeholders until they are confirmed.
