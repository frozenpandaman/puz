# HTML5 crossword puzzle reader

Modified version of the [CrosswordNexus HTML5 Crossword Solver](https://github.com/crosswordnexus/html5-crossword-solver) to look & function more like the [NYT Crosswords site](https://www.nytimes.com/crosswords) and [Downforacross](https://github.com/downforacross/downforacross.com).

Runs locally in your browser; no files are sent to the server.

The following file formats are supported:

- **.ipuz** [open format] (JSON) – [info](http://www.ipuz.org/), [more info](http://fileformats.archiveteam.org/wiki/IPUZ) _(partial, crossword-style only)_
- **.puz** [Across Lite] (binary file) – [info](https://code.google.com/archive/p/puz/wikis/FileFormat.wiki), [more info](http://fileformats.archiveteam.org/wiki/PUZ_(crossword_puzzles)), [even more info](https://www.litsoft.com/across/docs/AcrossTextFormat.pdf)
- **.jpz** [Crossword Compiler] (XML) – [info](http://crossword.info/docs/puzzle.xsd.html)
- **.cfp** [CrossFire] (XML)


### Caveats/bugs

 - "Check" function will not mark a square incorrect if its answer is a rebus
 - Word highlighting malfunctions in (very rarely-used) unchecked/unnumbered 1x1 squares
 - Shaded squares are not supported when viewing .puz files

---

#### File format-related resources

 * [.puz → .jpz converter #1](https://jpd236.github.io/kotwords/crossword.html) (web app)
 * [.puz → .jpz converter #2](https://github.com/crosswordnexus/crossword-tools/blob/main/jscrossword/index.html) (downloadable HTML file)
 * [.jpz → .ipuz converter](https://sourceforge.net/p/jpz2ipuz/code/HEAD/tree/jpz2ipuz.pl) (downloadable Perl script)