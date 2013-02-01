GRID COURSE FORMAT
============================
Package tested in: moodle 2.3+

QUICK INSTALL
==============
Download zip package, extract the grid folder and upload this folder into course/format/.

FILES
--------------

* grid/format.php

  Code that actually displays the course view page.

* grid/config.php

  Configuration file, mainly controlling default blocks for the format.

* grid/lang/en/format_grid.php
* grid/lang/ru/format_grid.php

  Language file containing language strings for grid format.

  Note that existing formats store their language strings in the main
  moodle.php, which you can also do, but this separate file is recommended
  for contributed formats.

  Of course you can have other folders as well as just English and Russian
  if you want to provide multiple languages.

* grid/db/install.xml

  Database table definitions.

* grid/db/upgrade.php

  Database upgrade instructions.

* grid/version.php

  Required for using database tables. The file provides information 
  about plugin version (update when tables change) and required Moodle version.

* grid/styles.css

  The file include in the CSS Moodle generates.

* grid/backuplib.php
  grid/restorelib.php

  Backup and restore run automatically when backing up the course.
  You can't back up the course format data independently.

ROADMAP
=============

* add new options screen to allow setting a few things:
  - specify overlay icon behaviour (no overlay, new changes, not started, topic completed)
  - specify position of label text (over, under, hover/tap caption)
  - specify image size
* fix overlay to work better in more browsers, particularly tablets
* fix bodgy css box layout for images
* 
