# jekyll-spin
A Bash script to automatically spin up a jekyll site from a designated repo.

This script:
 - Creates a new directory for a Jekyll site in /var/www.
 - Installs node & bower dependencies.
Ubuntu: add this script to /usr/local/bin
Make it executable, then you can invoke it by typing "jekyll-spin" in the terminal.

The script is optimized for this repo: git@bitbucket.org:RoryEgan/generic-new.git,
but it will work for any jekyll site that contains a Gruntfile, a package.json
and a bower.json.

The script clones the repo into the /var/www directory, then renames the cloned
directory into a name that you have been prompted to input.
