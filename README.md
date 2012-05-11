ts-krinkle-mwSnapshots
======================

## Install:
* Create cache directory (chmod 755)
* Create logs directory
* Create local.php
* Create remotes directory
* Inside the remotes directory, run:<br>
  `git clone https://gerrit.wikimedia.org/r/p/mediawiki/core.git mediawiki-core`
* Run updateSnaphots.php
* Symlink ./cache/snapshots to ./public_html/snapshots
* Schedule updateSnaphots.php to run hourly<br>
   `0 * * * * php $HOME/externals/ts-krinkle-mwSnapshots/scripts/updateSnaphots.php > $HOME/externals/ts-krinkle-mwSnapshots/logs/updateSnaphots.log 2>&1`
* Symlink ./public_html to ~/public_html/mwSnapshots
