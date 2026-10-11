# Building Assets 3D – Service Cloud V2 mashup

Single self-contained file: `index.html` (three.js, SAP 72 fonts, icons and design tokens are all inlined – no external requests).

## Deploy
1. Commit `index.html` to the repo root (or `docs/`).
2. Host it (GitHub Pages, SAP BTP, any static host) over **HTTPS**.
3. In SSC V2 create an HTML mashup pointing to the hosted `index.html` URL.

Clicking service call **56770** sends `window.parent.postMessage({operation:"navigation", params:{objectKey, routingKey:"case", viewType:"details"}}, "*")` to open the case in SSC V2.
