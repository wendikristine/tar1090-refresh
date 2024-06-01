Sadly, this is a dead fork.

# Content for prod team can be found found in three places

### 1. On the `master` branch, in the `PROD_ASSETS` root-level folder

  - Icons - self-explanatory. note that each SVG file will look empty because the icons are white against a transparent background
  - Graphics - created additional versions of the altitude legend.
     - vertical, useful for mobile?
     - map dark mode with white instead of black. I also considered a script that would change the black HEX to white HEX in the SVG when the user selects a dark map. 
  - HTML/CSS - self-explanatory. For an easy diff, see [PR301](https://github.com/wiedehopf/tar1090/pull/301)
  - Misc

### 2. dev work in context, phase 1: `clean-up-before-real-work` branch

  - Organized style.css into the site’s component parts: root and shared elements, map controls, infoblocks, sidebar, sidebar components, settings panel, replay bar, and library CSS file overrides (jQuery, open-layer, layer-switcher, font-awesome)
  - Added Font Awesome v5.14.4 library via CDN - no storage increase, no performance impacts, free and not tied to any account
  - Modified the jQuery CSS files via the ThemeRoller to better align with light v. dark mode inversions and included brand colors; modifications to the site from these modifications will be included in a future PR

![Phase1](https://github.com/wendikristine/tar1090-refresh/assets/19353299/70461c14-d9a3-4853-813b-24dc413e5d6a)

### 3. dev work in context, phase 2: `map-controls` branch, although work was not complete

  - Updated script.js to change the way the sidebar show/hide buttons work and added icons dynamically based on the state of the sidebar
  - Grouped and restyled map control buttons, appropriate for all screen sizes, a step in the right direction regarding accessibility
  - Added a sticky header to the sidebar

![Phase2](https://github.com/wendikristine/tar1090-refresh/assets/19353299/60a44d8c-ce1a-464a-9d2b-13a73a3bfa4f)
