# DocCompare image spec

Every image the screens need, with size, content and where it is used. Paths are relative to `doccompare/images/`.

**Status:** no JPG photos exist yet. Only the three SVG files in the last section are present. Until a photo exists, the browser shows the fallback: a green-to-forest background, with initials for doctor photos.

Screen numbers below match the file names in `screens/` (for example `05` is `05-home.html`).

## Doctor photos (`doctors/`)

Size for all: **400 x 400 px, square, JPG**. Face centred, plain light background, shown with `object-fit: cover`.

| File | Doctor | Gender | What the photo shows | Fallback initials | Used on |
|---|---|---|---|---|---|
| `doctors/rao.jpg` | Dr. Anaya Rao | Female (screen 11 uses "she") | Calm, friendly portrait. Smiling, relaxed, business-casual or white coat. | AR | 05, 06, 10, 11, 12, 13, 14, 15, 16, 18, 22, 23, 24, 26, 27 |
| `doctors/desai.jpg` | Dr. Kabir Desai | Male (confirm) | Professional portrait. Friendly expression, white coat or dark blazer. | KD | 05, 10, 14 |
| `doctors/shah.jpg` | Dr. Meera Shah | Female (confirm) | Professional portrait. Confident, approachable, white coat or dark blazer. | MS | 06, 10, 14, 15, 16, 23 |
| `doctors/iyer.jpg` | Dr. Mira Iyer | Female (confirm) | Professional portrait. Warm expression, white coat or dark blazer. | MI | 05, 10, 14, 15, 16, 23 |
| `doctors/joshi.jpg` | Dr. Arjun Joshi | Male (confirm) | Professional portrait. Friendly expression, white coat or dark blazer. | AJ | Not yet. Screens 10 and 14 show initials only. |
| `doctors/qureshi.jpg` | Dr. Salman Qureshi | Male (confirm) | Professional portrait. Friendly expression, white coat or dark blazer. | SQ | Not yet. Screens 10 and 14 show initials only. |

**Standard names:** every screen and this file use the names above. `joshi.jpg` and `qureshi.jpg` are the file names for Arjun Joshi and Salman Qureshi.

## Clinic photo (`clinics/`)

| File | Size | What the photo shows | Used on |
|---|---|---|---|
| `clinics/sunrise.jpg` | 800 x 400 px, wide, JPG | Bright, clean reception or entrance of Sunrise Heart Clinic. Cropped with `object-fit: cover`. | 13 |

## Hero and banner images (`hero/`)

| File | Size | What the image shows | Used on |
|---|---|---|---|
| `hero/welcome.jpg` | 800 x 1000 px, portrait, JPG | Friendly doctor with a patient. Keep faces in the upper-middle area because the banner is cropped at the bottom. | 02 |
| `hero/auth-banner.jpg` | 780 x 400 px, wide, JPG | Calm clinic scene, low contrast so the white logo and text read clearly. | 03, 04 |
| `hero/home-banner.jpg` | 700 x 320 px, wide, JPG | Stethoscope or heart-care scene. | 05 |

## Existing vector files (no action needed)

| File | Size | What the file shows | Used on |
|---|---|---|---|
| `logo.svg` | 88 x 88 px | Logo mark: forest rounded square with gold heart-pulse. | Reference asset |
| `pattern.svg` | 390 x 844 px | Splash background: gold plus grid and rings at 12% opacity. | 01 |
| `map-sunrise.svg` | 350 x 180 px | Illustrated map with a gold-ringed forest pin. | 13 |

## Fallback rules

- Doctor photos: each uses a `photo` wrapper with a `photo__initials` span behind the `<img class="photo__image">`. Keep the wrapper for every new photo.
- Banners (`banner__image`) on 02, 03, 04, 05 and 13 have no initials or colour fallback. If a banner file is missing, the area shows only the page background.

## Summary: files to add

- 6 doctor photos (`doctors/`), 400 x 400 px each
- 1 clinic photo (`clinics/sunrise.jpg`), 800 x 400 px
- 3 hero images (`hero/`): welcome 800 x 1000, auth-banner 780 x 400, home-banner 700 x 320

Total: 10 JPG files.
