# HTML5 crossword puzzle player

Modified version of the [CrosswordNexus HTML5 Crossword Solver](https://github.com/crosswordnexus/html5-crossword-solver) to look & function more like the [NYT Crosswords site](https://www.nytimes.com/crosswords) and [Downforacross](https://github.com/downforacross/downforacross.com), with added mobile support and more.

Runs locally in your browser; no files are sent to the server.

The following file formats are supported:

 - **.ipuz** [open format] (JSON) – [info](http://www.ipuz.org/), [more info](http://fileformats.archiveteam.org/wiki/IPUZ) _[partial, crossword-style only]_
 - **.puz** [Across Lite] (binary file) – [info](https://code.google.com/archive/p/puz/wikis/FileFormat.wiki), [more info](http://fileformats.archiveteam.org/wiki/PUZ_(crossword_puzzles)), [even more info](https://www.litsoft.com/across/docs/AcrossTextFormat.pdf)
 - **.jpz** [Crossword Compiler] (XML) – [info](http://crossword.info/docs/puzzle.xsd.html)
 - **.cfp** [CrossFire] (XML) _[only with no blank squares]_


### Caveats

 - No support for clue references/continuations (secondary highlight)
 - Rebus bugs:
   - Puzzle will be marked as solved if all squares except rebuses are correct, and rebus squares will be changed to show answers
   - "Check" function will not mark a square incorrect if its answer is a rebus
   - Non-blank squares which contain a rebus as the solution (whether filled in as such or not) will not change to the solved color upon revealing the puzzle solution
 -  & do not show as the "revealed" color
 - Shaded squares (colored backgrounds) are not supported in .puz format
 - Word highlighting malfunctions in (very rarely-used) unchecked/unnumbered 1x1 squares

---

#### File format-related resources

 * [.puz → .jpz converter #1](https://jpd236.github.io/kotwords/crossword.html) (web app)
 * [.puz → .jpz converter #2](https://github.com/crosswordnexus/crossword-tools/blob/main/jscrossword/index.html) (downloadable HTML file)
 * [.jpz → .ipuz converter](https://sourceforge.net/p/jpz2ipuz/code/HEAD/tree/jpz2ipuz.pl) (downloadable Perl script)