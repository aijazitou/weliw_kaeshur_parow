# weliw-kaeshur-parow

Let's Read Kashmiri (ؤ لِو کٲشُر پَرٛو), Part 1 (گۅڈنُیک حصہٕ)

A children's Kashmiri alphabet and reading book, written in plain HTML and CSS. It is designed to be read on phones and laptops, and to be printed as a 7 × 10 inch book.

> Work in progress. Some chapters are still empty and some pages contain sample content. Expect things to change.

## Credits

- Authors: غۅلام رسوٗل عِرفان تہٕ اعجاز ٳتۍ
- Illustrations (نقاش): اقصٰی اعجاز

## What is in this repository

| File | What it is | Status |
|---|---|---|
| `index.html` | Cover, introduction and list of chapters | In progress |
| `01-alphabet.html` | The alphabet, six letters per page, with pictures | In progress |
| `02-consonants.html` | All 42 letters in one grid, and the consonants table | In progress |
| `03-vowels.html` | Vowel marks (زَبر زیر) | Empty |
| `04-basics.html` | Basic sentences, days, months, riddles | Empty |
| `05-advanced.html` | Stories, poems and essays | Empty |
| `style.css` | All the styling, shared by every page | In progress |

Two folders are also needed:

- `fonts/` holds the font file `GulmargNastaleeq.ttf`.
- `diagrams/` holds the pictures used on the alphabet pages (for example `1001_al.jpg`).

## How to view the book

1. Download or clone this repository.
2. Make sure the `fonts` and `diagrams` folders are next to the HTML files.
3. Open `index.html` in a web browser. The chapter links on that page open the other files.

No build step or internet connection is needed.

## How to print or make a PDF

Each chapter file is exported separately.

1. Open the chapter in Chrome.
2. Choose Print, then set the destination to "Save as PDF".
3. Set Margins to "None" and turn on "Background graphics".

The page size (7 × 10 in) is set in `style.css`.

## How to add a new page

1. Copy `99-sample.html` and rename the copy.
2. Replace the `<!-- REPLACE -->` comment with the page content.
3. Update the header text, the book name and the page number.

Each page is one `<div class="page">` block. Repeat the block for more pages.

## Colors

All the colors are variables in the `:root` block at the top of `style.css`. Change a value there and the whole book updates. The palette is inspired by Kashmir: Dal Lake blue, chinar-leaf gold and chinar red. The letter cards stay white on purpose so they blend into the white edges of the pictures.

The five chapter boxes on `index.html` have their colors written directly in the HTML.

## Planned

- Automatic page numbering (page numbers are typed by hand for now)
- Extra margin on the binding side for the printed version
- The remaining chapters

## License

To be decided. Until a license is added, all rights are reserved.

The font file has its own license. Check that it allows redistribution before publishing it here.
