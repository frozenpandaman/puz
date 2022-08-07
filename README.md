# HTML5 crossword puzzle player

Modified version of the [CrosswordNexus HTML5 Crossword Solver](https://github.com/crosswordnexus/html5-crossword-solver) to look & function more like the [NYT Crosswords site](https://www.nytimes.com/crosswords) and [Downforacross](https://github.com/downforacross/downforacross.com), with added mobile support and more.

Runs locally in your browser – no data is uploaded online.

The following file formats are supported:

 - **.ipuz** [open format] (JSON) – [info](http://www.ipuz.org/), [more info](http://fileformats.archiveteam.org/wiki/IPUZ)
 - **.puz** [Across Lite] (binary file) – [info](https://code.google.com/archive/p/puz/wikis/FileFormat.wiki), [more info](http://fileformats.archiveteam.org/wiki/PUZ_(crossword_puzzles)), [even more info](https://www.litsoft.com/across/docs/AcrossTextFormat.pdf)
 - **.jpz** [Crossword Compiler] (XML) – [info](http://crossword.info/docs/puzzle.xsd.html)
 - **.cfp** [CrossFire] (XML) _(only if no blank squares exist)_

### Added support in this fork
- Cells with multiple answers (Schrödinger cells)
- Checking/revealing cells with rebuses

### Caveats

 - No support for clue references/continuations (secondary highlight)
 - Shaded squares (colored backgrounds) are not supported in .puz format
 - Word highlighting malfunctions in (very rarely-used) unchecked/unnumbered 1x1 squares

---

#### File format-related resources

 * [.puz → .jpz converter #1](https://jpd236.github.io/kotwords/crossword.html) (web app)
 * [.puz → .jpz converter #2](https://github.com/crosswordnexus/crossword-tools/blob/main/jscrossword/index.html) (downloadable HTML file)
 * [.jpz → .ipuz converter](https://sourceforge.net/p/jpz2ipuz/code/HEAD/tree/jpz2ipuz.pl) (downloadable Perl script)