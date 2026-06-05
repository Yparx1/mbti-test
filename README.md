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
The original uploaded file is included as `index_original_backup.html`.
The source grid is included as `source_grid.jpeg`.


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
