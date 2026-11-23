# Editing Guide

Open `index.html` in any text editor (Notepad, VS Code). Use Find (Ctrl+F) to jump to the names below.
Save, then refresh the browser to see changes.

## 1. Your WhatsApp number
Find `const WA=`. Replace the dummy number with yours: country code, no `+`, no spaces.
Example (Pakistan): `const WA="923001234567";`

## 2. Product names, categories and prices
Find `const P=[`. Each product is one row:

`["Product name","Category",price,"#colour","shape"]`

- Category must be one of: `Bridal`, `Formal`, `Party`, `Casual`, `Winter`, `Abaya`, `Kids`, `Men`, `Dupatta`
- Price is a plain number (no commas), in PKR
- The colour and shape only matter for products that have no photo

The order of the rows matters: each product has an id equal to its position, starting at 0.
`docs/products.csv` shows every id, name, price and photo file.

## 3. Product photos
Find `const IMG=`. It maps a product id to a photo file, for example:

`"0": "images/products/00-maroon-and-gold-bridal-set.jpg"`

To replace a photo, drop a new image into `images/products/` and change the path for that id.
Tip: use portrait photos about 440 x 640 pixels so the page loads fast.

## 4. Adding a new product
1. Add a new row to `const P=[...]`. Put it at the END of the list so the other ids do not change.
2. Add its photo file to `images/products/`.
3. Add `"95": "images/products/your-photo.jpg"` to `const IMG=` (use the new product's id).

## 5. Animations
- Title-page animation: `images/hero/frame-01.jpg` to `frame-49.jpg`
- Party Maxi twirl: `images/party-maxi/frame-01.jpg` to `frame-20.jpg`
Replace frames with the same file names to change the animations. Speed is set by the numbers `85` (hero) and `110` (party maxi) near the end of the file; smaller means faster.

## 6. Colours
Find `html:root:root:root{`. The main colours are `--bg` (background), `--fg` (text), `--accent` (gold), `--card` and `--line`.

## 7. Wording and Urdu translation
Find `const D=`. It holds the English (`en`) and Urdu (`ur`) text for headings, buttons and category names.
