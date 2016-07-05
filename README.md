# jekyll-spin
A Bash script to automatically spin up a jekyll site from a designated repo. The jekyll site must use Node.js, Grunt and Bower. The repo of a good example site to test the script on: https://github.com/RoryEgan/example-business-template

The script was made to speed up the cloning and setup process of jekyll sites that all have the same basic structure regarding usage of Grunt, Bower etc. As such it requires a fairly specific structure in the repository to be cloned.

This script:
 - Creates a new directory for a Jekyll site in /var/www/html.
 - Installs node & bower dependencies.
 - Optionally creates a GitHub repo for the project.
 - Optionally runs the grunt default task.


Ubuntu: add this script to /usr/local/bin using a symlink
Make it executable, then you can invoke it by typing "jekyll-spin" in the terminal.


The script clones the repo into the /var/www/html directory, then renames the cloned
directory into a name that you have been prompted to input. All iterances of the old name are changed throughout the site, so
the baseurl etc. should be correct for the new project name.
