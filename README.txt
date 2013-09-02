
CONTENTS OF THIS FILE
---------------------

* Overview
* Features
* Requirements
* Known problems
* Version history
* Future plans
* Similar projects
* Credits

OVERVIEW
--------

This module aims to make Github's Emoji smileys available in Drupal through the
Smiley module.

FEATURES
--------

* Auto-detects the smileys published in Github's gemoji library, and tells the
  smiley module where to find them.
* Uses the Emoji codes documented on the Emoji cheat sheet at
  http://www.emoji-cheat-sheet.com/

REQUIREMENTS
------------

* The Smiley module, version 7.x-2.x or better, available from:
  https://drupal.org/project/smiley
* Github's gemoji library, available from:
  https://github.com/github/gemoji/releases

KNOWN PROBLEMS
--------------

I don't know of any problems at this time, so if you find one, please let me
know by adding an issue!

VERSION HISTORY
---------------

The 1.x branch provides the Smiley module with the Emoji available in the gemoji
library.

FUTURE PLANS
------------

Since this module auto-detects the smileys in the library it integrates with, it
might already do everything it needs to! However, if there are changes to the
gemoji library that stop it from working, I'll make the necessary changes.

Once the Smiley module is available for Drupal 8, I'll port this module.

SIMILAR PROJECTS
----------------

I'm not aware of any modules similar to this one.

CREDITS
-------

Concept by mparker17 and Rob Loach. Special thanks to fizk for allowing me to
help make the Smiley module better.

Thanks to the Japanese Telecoms for inventing Emojis, the Unicode Consortium for
including Emojis in the Unicode standard, Apple for creating a widely-available,
widely-distributed Emoji font, and Github for their gemoji library.
