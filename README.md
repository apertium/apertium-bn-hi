# Bengali and Hindi: apertium-ben-hin

This is an Apertium language pair for translating between Bengali and
Hindi. What you can use this language package for:

* Translating between Bengali and Hindi
* Morphological analysis of Bengali and Hindi
* Part-of-speech tagging of Bengali and Hindi

For information on the latter two points, see subheading "For more
information" below

## Requirements

You will need the following software installed:

* lttoolbox (>= 3.3.0)
* apertium (>= 3.3.0)
* vislcg3 (>= 0.9.9.10297)
* apertium-ben
* apertium-hin

If this does not make any sense, we recommend you look at: www.apertium.org

## Compiling

Given the requirements being installed, you should be able to just run:

    $ ./configure
    $ make
    # make install

You can use `./autogen.sh` instead of `./configure` in case you're compiling from
source. If you installed any prerequisite language packages using a --prefix
to ./configure, make sure to give the same --prefix to ./configure here.

## Testing

If you are in the source directory after running make, the following
commands should work:

    $  echo "TODO test sentence 1" | apertium -d . ben-hin
    TODO test translated sentence 1

    $ echo "TODO test sentence 2" | apertium -d . hin-bin
    TODO test translated sentence 2

After installing somewhere in $PATH, you should be able to do e.g.

    $  echo "TODO test sentence 1" | apertium ben-hin
    TODO test translated sentence 1

## Files and data

* apertium-ben-hin.ben-hin.dix  - Bilingual dictionary
* apertium-ben-hin.ben-hin.t1x  - Chunking rules for translating into Hindi
* apertium-ben-hin.hin-bin.t1x  - Chunking rules for translating into Bengali
* apertium-ben-hin.ben-hin.t2x  - Interchunk (stage 1) rules for translating into Hindi
* apertium-ben-hin.hin-bin.t2x  - Interchunk rules for translating into Bengali
* apertium-ben-hin.ben-hin.t3x  - Interchunk (stage 2) rules for translating into  Hindi
* apertium-ben-hin.hin-bin.t3x  - Postchunk rules for translating into Bengali
* apertium-ben-hin.ben-hin.lrx  - Lexical selection rules for translating into  Hindi
* apertium-ben-hin.hin-bin.lrx  - Lexical selection rules for translating into Bengali
* modes.xml                     - Translation modes
* bengali_sentiment_analysis.ipnyb

## For more information

* http://wiki.apertium.org/wiki/Installation
* http://wiki.apertium.org/wiki/apertium-ben-hin
* http://wiki.apertium.org/wiki/Using_an_lttoolbox_dictionary

## Help and support

If you need help using this language pair or data, you can contact:

* Mailing list: apertium-stuff@lists.sourceforge.net
* IRC: #apertium on irc.freenode.net

See also the file AUTHORS included in this distribution.
