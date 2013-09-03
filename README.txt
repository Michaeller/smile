
CONTENTS OF THIS FILE
---------------------

* Overview
* Features
* Requirements
* Installation
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

INSTALLATION
------------

1. Download and install the gemoji library.

   Download the latest release of the gemoji library from
   https://github.com/github/gemoji/releases -- the files are available in
   .tar.gz and .zip formats and can be extracted using most compression tools.
   At the time of writing, the most-recent version is 1.4.0, but newer versions
   of gemoji should work if the file structure is similar to 1.4.0.

   Extract the gemoji library. This will create a new directory, gemoji-x.y.z/,
   where x.y.z is the version number you downloaded.

   Rename the directory to gemoji/.

   Then, move it inside the sites/all/libraries/ in your Drupal site. You may
   need to create the libraries/ folder. At this point, the gemoji.gemspec file
   will be at /path/to/drupal/docroot/sites/all/libraries/gemoji/gemoji.gemspec.

   See https://drupal.org/node/1440066 for further information.

2. Download and install the smiley_emoji project.

   Install as usual, see http://drupal.org/node/70151 for further information.

3. Ensure that Drupal recognizes the gemoji module.

   In a web browser, log in as the user you created when you set up the site
   (user/1) and go to Administration -> Reports -> Status report. For instance,
   if your Drupal website is accessible at http://example.com, the status report
   will be at http://example.com/admin/reports/status.

   Look for a line in the status report titled "Gemoji library". If the version
   of gemoji you downloaded is listed next to it, then the library is installed
   correctly. If an error is reported, please refer to
   https://drupal.org/node/1440066 for further information.

4. Add the smiley filter to a text format.

   Go to Administration -> Configuration -> Content authoring -> Text formats.

   You will see one or more text formats listed, typically Filtered HTML, Full
   HTML and Plain text. Click the "configure" link in the Operations column next
   to the text format you want to enable smileys in.

   You will see the text format configuration screen. Under "Enabled filters",
   check "Convert smileys to images". In the Filter processing order section,
   ensure "Convert smileys to images" is placed below "Limit allowed HTML tags".
   Otherwise, your smileys may not show up.

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
