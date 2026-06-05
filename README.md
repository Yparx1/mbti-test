# MBTI portrait icon pack

Upload this folder structure to your GitHub Pages project:

```
index.html
icons/
  people/
    queen-elizabeth-ii.png
    warren-buffett.png
    ...
```

The modified `index.html` already uses the portrait images in the result screen.


Update: Removed em dashes from intro text and kept bullet points in strengths/watch-for sections.


Updated icon crops were replaced from the user-provided borderless source grid.


Update: person result cards now show a small title line under each portrait name.


Bug fix: corrected portrait image path lookup from personImagePaths to personPortraits.


## Added interaction effects

- Opening loading screen with the title and “made by Yparx1”
- Buttons expand slightly on hover
- Light tone plays when buttons are clicked
- Soft bell sound plays when the quiz result appears
- No sound toggle was added

Note: browsers require the first user interaction before audio can play, so the click and finish sounds activate after the user interacts with the page.


## Favicon

Added a cute browser-tab favicon using:
- `favicon.svg`
- `favicon.ico`
- `favicon-32.png`
- `apple-touch-icon.png`
- `icon-512.png`


## Type icons

The main result icons are now minimalist inline SVG symbols, not PNG files. Edit them in `index.html` inside the `typeIcons` object.


## Custom button sounds

Different tones are now used for:
- Begin / Start
- Back
- Next
- Retake
- See result

The finish/result screen still plays the soft accomplishment bell.


## Audit and cleanup

This version was reviewed and cleaned up.

What was checked:
- JavaScript syntax
- 20-question quiz flow
- intro → questions → result → retake flow
- result rendering for all 16 types
- all portrait image paths used by results
- custom audio routing for Begin, Back, Next, See result, and Retake
- selection auto-advance behavior

Fixes included:
- Added a safe auto-advance timer so selecting an answer cannot skip or get stuck if the user clicks quickly.
- Cleared pending auto-advance timers when using Back, Next, See result, or Retake.
- Reset the finish bell state on Begin and Retake.
- Prevented disabled buttons from playing sounds.
- Removed unused backup/source files from the final package.


## Loading timing update

- Beginning loading screen now lasts 3 seconds.
- Pressing **See result** now shows a 2-second result loading screen before the result appears.


## Icon cleanup

The result type icons were revised into cleaner, more balanced minimalist inline SVG symbols.
They remain editable inside `index.html` in the `typeIcons` object.


## Premium MBTI / type icon revision

Updated the type icons to be more premium and consistent:
- INTJ changed from knight to a compass/architect icon
- ISTP changed from wrench to a piano key to better fit Virtuoso
- ENFP, INFP, ESTP, ESFP, ENTJ, and INTP kept their stronger concept directions
- all icons now use simple black outline SVG
- same stroke thickness
- same visual weight
- same size box
- reduced overly detailed or mismatched styling


## Type icon style update

Updated the result type icons to:
- remove the circular border/frame
- keep the clean inline SVG outline style
- add a subtle soft shadow for a more premium look


## PNG MBTI / type icons

The result type symbols now use neat centered PNG files with transparent backgrounds.

Files are in:
- `icons/types/intj.png`
- `icons/types/intp.png`
- ...
- `icons/types/esfp.png`

They were cropped from the approved icon set, cleaned, centered on transparent canvases, and wired into `index.html`.


## Type icon fix

Replaced the MBTI/type icon PNGs with the uploaded full versions from `types.zip`.

Also adjusted the result icon container so icons are:
- fully visible
- centered
- not clipped
- transparent background


## Type icons rebuilt from full grid

The MBTI/type icons were rebuilt from the complete 4x4 grid image provided by the user.

This version:
- crops exact 4x4 cells from the full image
- removes the checkerboard/light background
- keeps the full icon shape
- centers each PNG on a transparent 256x256 canvas
- avoids cutting edges
- includes `type-icons-preview.html` for checking the icons
