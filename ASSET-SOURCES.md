# Asset sources

Every SVG in `assets/` is self-contained: photos, icons and fonts are embedded inline, and none of the SVGs makes a network request when it renders.

## Photos

| File | Source | Treatment |
| :-- | :-- | :-- |
| `hero.svg`, `id-dashboard.svg` | `id.png` (supplied by Pronov Mazumdar) | Scaled to 640 px and 420 px wide with Lanczos resampling and embedded as PNG. Original alpha kept; no masks or retouching. Hero crops the bottom edge to the stage card. |
| `connect.svg` | `right_pointing.png` (supplied by Pronov Mazumdar) | Scaled to 560 px wide and embedded as PNG. Original alpha kept. |

## Fonts (SIL Open Font License 1.1)

| Family in SVG | Font | Instance | Source |
| :-- | :-- | :-- | :-- |
| `PM Display` | Bricolage Grotesque | opsz 96, wdth 100, wght 800 | [google/fonts · ofl/bricolagegrotesque](https://github.com/google/fonts/tree/main/ofl/bricolagegrotesque) |
| `PM Text` | Bricolage Grotesque | opsz 14, wdth 100, wght 500 | same |
| `PM Mono` | JetBrains Mono | wght 500 | [google/fonts · ofl/jetbrainsmono](https://github.com/google/fonts/tree/main/ofl/jetbrainsmono) |

Each font is a static instance subset to Basic Latin plus a few punctuation marks and arrows, compressed to WOFF2 and embedded as base64. The licence texts are in `LICENSES/`. Neither font declares a Reserved Font Name.

## Icons

Simple Icons **v16.34.0** ([simple-icons/simple-icons](https://github.com/simple-icons/simple-icons), icon data CC0 1.0). Brand marks remain trademarks of their owners; see `LICENSES/SimpleIcons-DISCLAIMER.md`.

| Label | Mark used | Source |
| :-- | :-- | :-- |
| Python | Simple Icons `python` | python.org/community/logos |
| Java | Simple Icons `openjdk` (Duke, the OpenJDK mascot) | Oracle licenses its Java cup logo only through a logo programme, and Simple Icons doesn't carry it. The OpenJDK mark comes from hg.openjdk.java.net/duke. |
| TypeScript | Simple Icons `typescript` | typescriptlang.org/branding |
| SQL | Generic database glyph, drawn for this project | SQL is a language standard with no brand mark. |
| PyTorch | Simple Icons `pytorch` | pytorch/pytorch.github.io logo.svg |
| LangChain | Simple Icons `langchain` | langchain.com |
| FastAPI | Simple Icons `fastapi` | tiangolo/fastapi docs icon |
| React.js | Simple Icons `react` | facebook/create-react-app logo |
| Node.js | Simple Icons `nodedotjs` | nodejs.org/en/about/branding |
| GCP | Simple Icons `googlecloud` | cloud.google.com |
| Power BI | Official Microsoft Power BI icon (`SVG/Power-BI.svg`) | [microsoft/PowerBI-Icons](https://github.com/microsoft/PowerBI-Icons), © Microsoft, **CC BY 4.0** (`LICENSES/CC-BY-4.0-PowerBI-Icons.txt`). Unmodified apart from namespacing its internal ids. |
| GitHub | Simple Icons `github` | github.com/logos |
| X | Simple Icons `x` | x.com |
| LinkedIn | Official LinkedIn [in] bug (`LI-In-Bug.png`) | [brand.linkedin.com/downloads](https://brand.linkedin.com/downloads), file `in-logo.zip`. Simple Icons removed LinkedIn at LinkedIn's request. Shown at original colours and aspect ratio, scaled only. |

When a brand colour has too little contrast against its chip, that icon uses its monochrome variant (dark on light chips, off-white on dark chips).

## Data

The ID dashboard figures were captured on 8 Oct 2026 (`Date` header of the response) from `https://api.github.com/users/pronov06` and `https://api.github.com/users/pronov06/repos`. They're a dated snapshot and don't update by themselves.
