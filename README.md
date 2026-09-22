# margins

A one-page site for **margins**, a fictional independent bookshop, built as a single
self-contained `index.html`: no build step, no framework, no bundler.

Live: https://dareos381.github.io/margins/

## What is in it

- A hand-written spring solver (react-spring's integrator), one shared ticker, scroll
  scrubs, clipped text reveals, digit rolls, pointer leans and a preloader.
- Smooth scrolling with Lenis; three.js for the 3D layers. Those two libraries are the
  only external code, pulled through an import map.
- Two WebGL layers written by hand: a thin-film-interference gradient behind the hero
  and the philosophy block, and a rigid-body field of loose pages with pointer push,
  page-on-page collisions and a scroll vortex.
- Every image is generated in the page itself: the books are procedural three.js
  geometry with covers, spines and page edges painted on canvas; the covers on the
  cards, the clock face, the brand stroke and the printer are CSS and SVG.
- The layout is written to a 1440 board in rem, with the root font size scaling with the
  viewport; below 1024 every block lays itself out in flow.
- `prefers-reduced-motion` removes the preloader, the leans, the page physics and the
  receipt feed.

## Running it

Open `index.html`, or serve the folder (`python3 -m http.server`) if your browser
restricts modules on `file://`.

## Credits

Names, addresses, titles and authors are invented. Type: Newsreader, Geist, Space Mono
and Allura via Google Fonts.
