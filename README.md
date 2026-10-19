# DocCompare

Clickable prototype of the DocCompare patient app (30 screens) and a doctor booking screen.

## Open the prototype

Open `index.html` in a browser. It lists every screen, grouped by flow. Each link opens a file in `screens/`.

## Folder layout

- `index.html`: screen index, the entry point.
- `screens/`: one HTML file per screen, numbered in the order a patient moves through the app.
- `css/`: `tokens.css` (colours, type, spacing), `base.css` (reset and typography), `components.css`, `screens.css`, `icons.css`.
- `images/`: logo and vector art, plus the photos listed in `images/IMAGE-SPEC.md`.

## Navigation

- Patient bottom nav (Home, Search, Visits, Profile) is on screens 05, 06, 22, 23 and 29. Each item links to its screen; the active item is marked with `aria-current`.
  - Home: `05-home.html`
  - Search: `06-search.html`
  - Visits: `23-appointments.html`
  - Profile: `29-profile.html`
- Doctor bottom nav (screen 30) only links Requests, which is the only doctor screen. Schedule, Patients and Profile are not linked because no screens exist for them yet.
- Tab bars at the top of the doctor and comparison screens link between their sections: `11`, `12`, `13` (doctor) and `15`, `16`, `17` (compare).
- `index.html` links to every screen.

## Images

Photos are not in the repo yet. Until they are added, each doctor photo shows its initials on a green background, and banners show only the page background. `images/IMAGE-SPEC.md` lists every image still needed, with size and content.

## Doctors

Doctor names are standardized across screens:

- Dr. Anaya Rao
- Dr. Kabir Desai
- Dr. Meera Shah
- Dr. Mira Iyer
- Dr. Arjun Joshi
- Dr. Salman Qureshi
