# Ideal EPUB Book

A collection of tips, tricks, and best practices I’ve learned over the years for creating EPUB ebooks.

## Background

I’ve often been frustrated by the lack of quality in EPUBs produced by otherwise reputable publishers. Nothing is more infuriating than paying good money for a book, only to find it riddled with issues like:

- Low-resolution images
- Poorly-parsed Table of Contents (e.g. ALL CAPS, improper nesting, duplicate entries, missing spaces)
- Images of text versus properly styled text/UTF-8 characters
- Zero support/thought of dark mode
- Hard-coded first-line capitalization/styling
- Small caps brute-forced with smaller font size instead of using `font-variant: small-caps`
- Poor implementation of drop-caps
- Spelling errors/typos
- Headings marked up as links back to the table of contents
- Footnotes marked up as links instead of using [EPUB footnote syntax](https://www.w3.org/TR/epub-ssv-11/#endnote) (to support pop-up UI)

## Tools

The following are super-helpful in EPUB production:

- [Sigil](https://sigil-ebook.com/sigil/) - Easily run EPUB validation, refactor to common folder structure, catch spelling issues, find unused CSS/files, etc.
- [EPUB Zip/Unzip](https://www.mobileread.com/forums/showthread.php?t=55681) - Quickly swap between zipped (production ready) and unzipped (editable) versions of your EPUB
- [epubcheck](https://github.com/w3c/epubcheck) - Official conformance checker for EPUBs.

## Resources

- Official Specs
  - [EPUB 3.3 W3C Spec](https://www.w3.org/TR/epub-33)
  - [EPUB 3 Structural Semantics Vocab 1.1](https://www.w3.org/TR/epub-ssv-11/)
  - [Dublin Core `dcterms`](https://www.dublincore.org/specifications/dublin-core/dcmi-terms/)
- [Accessible Publishing Knowledge Base](https://kb.daisy.org/publishing/docs/)  
  _Some useful guidance on semantics_
- [E-Production Resources](https://wiki.mobileread.com/wiki/E-Production)  
  _Community site for EPUB knowledge_
- [eBook Tricks](https://friendsofepub.github.io/eBookTricks/)  
  _Includes example html/css_
- iBooks
  - [Apple Books Asset Guide](https://help.apple.com/itc/booksassetguide/)  
    _Apple’s official guidance on how to best format EPUBs for iBooks_
- [Standard Ebooks](https://standardebooks.org/)  
  _Dedicated to producing the highest-quality EPUBs of public-domain literature._
  - [Producing an Ebook, Step by Step](https://standardebooks.org/contribute/producing-an-ebook-step-by-step)
    - [Manual of Style](https://standardebooks.org/manual/latest)
      - [The Structure of an Ebook](https://standardebooks.org/manual/latest/3-the-structure-of-an-ebook)
  - [High Level Structural Patterns](https://standardebooks.org/manual/latest/7-high-level-structural-patterns)
    - [Sectioning](https://standardebooks.org/manual/latest/7-high-level-structural-patterns#7.1)
    - [Headers](https://standardebooks.org/manual/latest/7-high-level-structural-patterns#7.2)
    - [Dedications](https://standardebooks.org/manual/latest/7-high-level-structural-patterns#7.3)
    - [Epigraphs](https://standardebooks.org/manual/latest/7-high-level-structural-patterns#7.4) _(quotes at beginning of chapters)_
    - [Poetry, verse, and song](https://standardebooks.org/manual/latest/7-high-level-structural-patterns#7.5)
    - [Plays and Drama](https://standardebooks.org/manual/latest/7-high-level-structural-patterns#7.6)
    - [Letters](https://standardebooks.org/manual/latest/7-high-level-structural-patterns#7.7)
    - [Images](https://standardebooks.org/manual/latest/7-high-level-structural-patterns#7.8)
    - [List of Illustrations (The LOI)](https://standardebooks.org/manual/latest/7-high-level-structural-patterns#7.9)
    - [Endnotes](https://standardebooks.org/manual/latest/7-high-level-structural-patterns#7.10)
    - [Glossaries](https://standardebooks.org/manual/latest/7-high-level-structural-patterns#7.11)
  - Semantic vocabulary
    - [EPUB 3 Structural Semantics](https://www.w3.org/TR/epub-ssv-11/)
    - [z3998 Semantics](https://www.daisy.org/z3998/2012/vocab/structure/)
    - [`se` Namespace](https://www.daisy.org/z3998/2012/vocab/structure/)
