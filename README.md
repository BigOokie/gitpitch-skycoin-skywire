# Skycoin-GitPitch-Decks

## Overview
This project has been established to maintain a GitPitch slide deck for the Skycoin project. The primary aim is to provide an accessable and factual source of information about Skycoin, Skywire, CX and the other numerous projects that fall under the Skycoin banner.

Inspiration for The GitPitch decks have been sourced from GitPitch and a handful of other sources, including:
- [Develop course and training materials using fruit punnets](https://hackernoon.com/develop-course-and-training-materials-using-fruit-punnets-cf9cfa88040f)
- [Intro to React.js GitPitch Deck](https://github.com/suddi/intro-to-react/)

## Using the Deck
If you want to use the Deck or parts of it, please feel free. Contributions back to the Deck are also welcome via GitHub PR. If you find issues please raise an issue in GitHub

The main Deck can be accessed publicly via the following URL:
https://gitpitch.com/bigookie/skycoin-gitpitch-decks/master/

### Deck Structure
The following outlines the Deck folder structure. This will assist in use and customisation of the Deck:

```
.
|-- assets                  (assets used by the deck - css, fonts, images, etc)
|   |-- css                 (Deck Theme CSS)
|   |-- fonts               (Deck Fonts)
|   |   `-- skycoin         (Official Skycoin Fonts)
|   `-- img                 (Image Assets - Keep these < 1MB)
|-- topics                  (Deck Topic Slides)
|   |-- 1-Start             (Start Slide)
|   |   `-- PITCHME.md
|   |-- 2-Project-Info      (Skycoin Project Information Slide)
|   |   `-- PITCHME.md
|   |-- 3-Presenter-Info    (Presenter Information Slide. Update this for your own use)
|   |   `-- PITCHME.md
|   |-- 4-Skycoin           (Skycoin Slide Deck)
|   |   `-- PITCHME.md
|   |-- 5-Skywire           (Skywire Slide Deck)
|   |   `-- PITCHME.md
|   |-- 6-CX                (CX Slide Deck)
|   |   `-- PITCHME.md
|   |-- 7-QA                (Q&A Slide Deck)
|   |   `-- PITCHME.md
|   `-- 8-End               (End Slide)
|       `-- PITCHME.md
|-- LICENSE
|-- PITCHME.md              (Main Deck Slide. Update this to include or exclude Slide topics)
|-- PITCHME.yaml            (Deck Theme Configuration)
`-- README.md               (This file)
```

### Customising the Deck
The Deck is designed to be modular and customisable. The content and primary flow of the Deck is controlled by the main `PITCHME.md` in the project root folder.

Currently the Deck includes each of the `topic` module Decks and appears like this:
```
---?include=topics/1-Start/PITCHME.md
---?include=topics/2-Project-Info/PITCHME.md
---?include=topics/3-Presentor-Info/PITCHME.md
---?include=topics/4-Skycoin/PITCHME.md
---?include=topics/5-Skywire/PITCHME.md
---?include=topics/6-CX/PITCHME.md
---?include=topics/7-QA/PITCHME.md
---?include=topics/2-Project-Info/PITCHME.md
---?include=topics/8-End/PITCHME.md
```

If you wanted to do a presentation on `CX` alone you could edit the main `PITCHME.md` to appear as follows - removing any of the `topic` module Decks that are not required:
```
---?include=topics/1-Start/PITCHME.md
---?include=topics/2-Project-Info/PITCHME.md
---?include=topics/3-Presentor-Info/PITCHME.md
---?include=topics/6-CX/PITCHME.md
---?include=topics/7-QA/PITCHME.md
---?include=topics/2-Project-Info/PITCHME.md
---?include=topics/8-End/PITCHME.md
```

Note that the following `topic` Decks were removed:
```
---?include=topics/4-Skycoin/PITCHME.md
---?include=topics/5-Skywire/PITCHME.md
```

You will also probably want to update the `3-Presenter-Info\PITCHME.md` to include your own details (as the presenter). The current file provides a reasonable template, but its your show - feel free to customise it to your needs.
```
## About Me

<div class="align-points">
	<i class="fa fa-telegram"></i> [@BigOokie](https://t.me/bigookie)<br/>
	<i class="fa fa-twitter"></i> [@BigOokie](https://twitter.com/BigOokie)<br/>
	<i class="fa fa-github"></i> [BigOokie](https://github.com/BigOokie)<br/>
</div>
```
**Note:** [Font Awesome](https://fontawesome.com/) is supported an provides the nice glyphs such as: `fa-globe`, `fa-github`, `fa-telegram`, `fa-github`