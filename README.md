# id-cards

A tiny, self-contained web page for showing ID cards (transit pass, membership card, ID, …)
fullscreen on your phone — e.g. to an inspector at the train station or mall entrance.

## Features

- **Add a card**: pick a photo/screenshot from your phone and give it a name.
- **Tap a card to show it fullscreen** on a black background. The screen is kept awake
  while it's shown (where the browser supports the Wake Lock API).
- **↻ Rotate** a landscape card to fill a portrait screen (remembered per card).
- **Swipe** left/right (or ‹ ›) to switch cards; tap to hide/show the buttons;
  back button / ✕ to close.
- **Private**: images are stored only on your phone in the browser's IndexedDB — nothing is uploaded.
- **Works offline** and can be installed with *Add to Home Screen*.

> Note: browsers can't keep a *link* to a file on your phone (they don't get access to file paths),
> so the page keeps its own copy of the image on the device instead.

## Usage

Host the folder on any static host (e.g. enable **GitHub Pages** for this repo:
Settings → Pages → Deploy from branch), open the URL on your phone, then
*Share → Add to Home Screen* (iPhone) or *⋮ → Add to Home screen / Install app* (Android).

On iPhone, Safari doesn't allow true fullscreen for web pages; opening the app from the
Home Screen icon removes the browser bars so the card fills the screen.

Opening `index.html#open` shows the first card immediately.
