# Pustika

Rearrange PDFs, photos of notes and text files for double-sided study printing. Runs entirely in the browser, so files are never uploaded.

## Supported files

- **PDF**: pages are copied as-is, so text stays sharp.
- **Photos** (JPG, PNG, WebP and anything else your browser can open; HEIC only in Safari): an optional cleanup whitens the paper and darkens the ink, removing shadows.
- **Text (.txt) and Markdown (.md)**: laid out to fit the chosen layout, so they print at exactly the text size you pick. Markdown headings, bold, italic, lists, quotes, code and tables are supported. Text in scripts like Hindi is drawn by the browser so it shows correctly.
- Pick several files to combine them in name order, or use **Add more files** to append.
- Word, PowerPoint and Excel files: export them to PDF first.

## Layouts

- **Booklet**: fold each session's sheets in half and staple. Best for books.
- **Pocket book**: quarter-size book, 4 pages per side. Cut the stack across the middle, put the bottom pile under the top, fold and staple. Best for text notes.
- **Flash cards**: 4 to 12 cards per sheet, with each back printed behind its front. Cut along the lines.
- **Cut and stack**: cut the printed stack in half and stack the piles. No folding.
- **2, 4 or 6 per side**: papers and notes (2), lecture slides (4 or 6).
- **Page and notes**: one page per side with ruled space for notes.
- **Notes sheet**: one page per side with note space you set up: beside the page, below it, or both, on portrait or landscape paper. Choose lines, dots, squares or blank, and how big the page is. Notes stay on the outer edge (mirrored on backs), and optional Cornell headings add "Questions" beside and "Summary" below.
- **1 per side**: full size, just selected and trimmed.

For spiral or punch binding, set a binding margin (1 per side, 2/4/6 per side, page and notes, notes sheet, cut and stack). It adds space on the left of fronts and the right of backs.

## Writing flash cards

Put cards in a .txt or .md file with an empty line between cards:

```
Q: Where do the light reactions happen?
A: In the thylakoid membranes.

Mitochondria :: Makes ATP for the cell

Krebs cycle
---
Happens in the matrix
- makes NADH and FADH2

Water splits at photosystem II
Oxygen is a by-product
```

- `Q:` and `A:` make a question card.
- `keyword :: meaning` makes a keyword card.
- A line of `---` splits the front from the back.
- Anything else is a note card with no back.
- Text is sized to fill each card. PDF pages and photos can also be cards, one per card or paired as front and back.

## Study features

- **Sessions**: split a PDF into chunks that each start on a fresh sheet, so you can print one at a time.
- **Recall page**: added at the end of each session, for writing what you remember before checking, with review boxes for spaced practice.
- **Margin trimming**: removes empty margins so text prints larger.

## Publish on GitHub Pages

1. Create a new public repository on GitHub, for example `pustika`.
2. Upload `index.html` (and this README) to the repository.
3. Go to **Settings > Pages**, set the source to **Deploy from a branch**, pick `main` and `/ (root)`, and save.
4. After a minute the app is live at `https://<your-username>.github.io/pustika/`.

## Printing tips

- Print double-sided with the flip setting the app shows (short edge for booklets and cut and stack).
- Keep the paper size the same as in the app, and print at actual size (100%).

Built with [pdf-lib](https://pdf-lib.js.org/) and [PDF.js](https://mozilla.github.io/pdf.js/).
