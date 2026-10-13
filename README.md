# Era Odyssey

**The companion website for Era Odyssey, a 2D idle combat game about Earth's geological history.** The game was created by a high school team for a learning technology competition. Players travel through geological periods, fight creatures, collect materials, craft equipment, and learn through an in-game book and timed questions.

> **Looking for the game systems, Unity architecture, or technical debt?** Read the [full game showcase and architecture guide in the Unity repository](https://github.com/jakkarin-promsee/Unity-EraOdesey/blob/main/README.md). This repository contains the separate website used to present the game, its story, creatures, artwork, and downloads.

[Game source and technical guide](https://github.com/jakkarin-promsee/Unity-EraOdesey) | [Full project archive on Google Drive](https://drive.google.com/drive/folders/16LznbdzYvz0Czip6VU_nDyZi0XOLzPTN?usp=sharing) | [Download page](assets/Play.html)

## About the game

Era Odyssey combines stage-based idle combat with educational content about geological time. The archived Unity source documents period and stage progression, enemy waves and bosses, four elemental skill trees, material drops, two-material crafting, equipment, save data, and the Book of Era quiz. The presentation build ran successfully; the Git repository is a partial source archive, while the complete project was stored on Google Drive because of its size.

For implementation details, code entry points, a gameplay flow diagram, restoration guidance, and a documented technical debt inventory, see the [Unity README](https://github.com/jakkarin-promsee/Unity-EraOdesey/blob/main/README.md).

## Website contents

| Page | Content |
| --- | --- |
| [Home](assets/Home.html) | Introduction and the story of Demain H. Cover, the research island Saxabra, and the Si-2505 device that sends him into Earth's past. |
| [Monster](assets/Monster.html) | Creature showcase. |
| [Information](assets/Information.html) | Educational and background material. |
| [Play](assets/Play.html) | Links to the game files and APK on Google Drive. |
| [Animation](assets/Animation.html) | Animation showcase. |
| [Gallery](assets/Gallery.html) | Game imagery organized by geological period. |
| [About](assets/About.html) | Team information. |

The site is built with static HTML, CSS, JavaScript, JSON, and image assets. The root [`index.html`](index.html) redirects visitors to `assets/Home.html` using JavaScript. Page navigation and asset URLs generally use `/assets/...` paths, so the site should be served from its repository root rather than opened as individual `file://` pages.

## Run the website locally

From the repository root, start a static file server, then open `http://localhost:8000/`:

```bash
python -m http.server 8000
```

This serves the root redirect and the `/assets/...` URLs used by the pages. The command requires Python; any static server that serves the repository root will also work. The website is independent of the Unity runtime.

## Project archives

- [Unity source repository](https://github.com/jakkarin-promsee/Unity-EraOdesey): game systems, architecture guide, and technical debt.
- [Original full-project Drive archive](https://drive.google.com/drive/folders/16LznbdzYvz0Czip6VU_nDyZi0XOLzPTN?usp=sharing): link preserved from the Unity repository's original `readme.txt`.
- [Website Play page](assets/Play.html): additional Drive and APK links as published on the companion site.

The current availability and contents of external downloads have not been verified in this documentation update. The repository preserves the website as a student project; its structure and content are documented here without implying that it is a current production release.
