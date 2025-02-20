# Ideal EPUB Book

A collection of tips, tricks, and best practices I’ve learned over the years for creating EPUB ebooks.

### Background

I’ve often been frustrated by the lack of quality in EPUBs produced by otherwise reputable publishers. Nothing is more infuriating than to pay good money for a book to then find it riddled with issues like:

- All headings marked up as links back to the table of contents
- Spelling errors
- Low-resolution images
- Images of text versus properly styled text/UTF-8 characters
- Hard-coded first-line capitalization/styling
- Poor implementation of drop-caps
- Small caps brute-forced with smaller font size instead of using `font-variant: small-caps`
- Footnotes marked up as links instead of using [EPUB footnote syntax](https://www.w3.org/TR/epub-ssv-11/#endnote) (to support UI like pop-ups)
- Poorly-parsed Table of Contents (e.g. ALL CAPS, improper nesting, duplicate entries)
