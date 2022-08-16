# In-browser crossword puzzle player

Modified version of the [CrosswordNexus HTML5 Crossword Solver](https://github.com/crosswordnexus/html5-crossword-solver) to look & function more like the [NYT Crosswords site](https://www.nytimes.com/crosswords) and [Downforacross](https://github.com/downforacross/downforacross.com), with added features.

**Link: [https://frozenpandaman.github.io/puz/](https://frozenpandaman.github.io/puz/)**

Alternatively, specify a file to load automatically using the `?file=myxw.ipuz` parameter at the end of the URL.

The following file formats are supported:

 - **.ipuz** [open format] (JSON) – [info](http://www.ipuz.org/), [more info](http://fileformats.archiveteam.org/wiki/IPUZ) **_(recommended!)_**
 - **.puz** [Across Lite] (binary file) – [info](https://code.google.com/archive/p/puz/wikis/FileFormat.wiki), [more info](http://fileformats.archiveteam.org/wiki/PUZ_(crossword_puzzles)), [even more info](https://www.litsoft.com/across/docs/AcrossTextFormat.pdf) _(no support for shaded squares)_
 - **.jpz** [Crossword Compiler] (XML) – [info](http://crossword.info/docs/puzzle.xsd.html)
 - **.cfp** [CrossFire] (XML) _(only if no unchecked squares exist)_

---

### Added in this fork
- [x] Mobile display & next/previous clue buttons
- [x] Clue references/continuations (secondary highlight)
- [x] Support for cells with multiple answers (Schrödinger squares)
- [x] Checking/revealing cells with rebuses
- [x] Option to highlight corresponding grid entries while mousing over clues in the clue list
- [x] Clues can be added for unchecked/unnumbered squares & navigation behaves correctly

### Missing features

 - [ ] Fading of sidebar clues when corresponding word is filled

---

#### File format-related resources

 * [.puz → .jpz converter #1](https://jpd236.github.io/kotwords/crossword.html) (web tool)
 * [.puz → .jpz converter #2](https://github.com/crosswordnexus/crossword-tools/blob/main/jscrossword/index.html) (downloadable HTML file)
 * [.jpz → .ipuz converter](https://sourceforge.net/p/jpz2ipuz/code/HEAD/tree/jpz2ipuz.pl) (downloadable Perl script)

#### Free crossword-related tools

 * Constructing
   * [Phil](https://www.jmviz.dev/Phil/) (jmviz fork with added features) &nbsp;•&nbsp; [CrossHatch](https://ben4808.github.io/) &nbsp;•&nbsp; [Crosshare](https://crosshare.org/construct) &nbsp;•&nbsp; [Crosserville](https://www.crosserville.com/)
   * [Crossword Grid Search](https://ugleh.com/gridsearch/)
 * Clueing & fill
   * [XWordInfo Finder](https://www.xwordinfo.com/Finder) &amp; [Clue Search](https://www.xwordinfo.com/SearchClues) &nbsp;•&nbsp; [cluer](https://tiwwdty.com/clue/) (Matt Ginsberg's clue database)
   * [Block Quarry](https://blockquarry.net/) &nbsp;•&nbsp; [OneLook Dictionary Search](https://www.onelook.com/) &nbsp;•&nbsp; [Qat](https://www.quinapalus.com/cgi-bin/qat)
 * Wordlists & tools
   * [spread the word(list)](https://www.spreadthewordlist.com/wordlist) &nbsp;•&nbsp; [Peter Broda's Wordlist](https://peterbroda.me/crosswords/wordlist/) &nbsp;•&nbsp; [Et Tu, Etui?](https://ettuetui.blogspot.com/2021/07/one-year-of-et-tu-etui.html) (memes) &nbsp;•&nbsp; [more](https://old.reddit.com/r/crossword/comments/nqsuku/all_the_downloadable_word_lists_ive_been_able_to/)
   * [Wordlisted](https://aaronson.org/wordlisted/)
 * Publication
   * [PDF generator](https://njyoon.github.io/pdf)
   * [Crossword Nexus Submission Checker](https://crosswordnexus.com/apps/submission_check/)
   * [Publication specs GSheet](https://docs.google.com/spreadsheets/d/12HGynb2VpJR2akQPT7iCMUBXxqcwzmk3kJjic8F24Kk/edit?usp=sharing)
