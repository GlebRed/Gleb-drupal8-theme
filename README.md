# Gleb twig theme for Drupal 8 based on Bootstrap 4  :watermelon:

### This is codebase for the course "Make Drupal 8 twig theme in 1h + useful tips"


##### As I'm using MAMP (on mac OS) to run a local server, here's my snippet from httpd.conf to set up an alias (to make Drupal run from http://localhost:8888/my-drupal8/).

MAMP for Windows and mac OS: https://www.mamp.info/en/

```
Alias /my-drupal8 "/Applications/MAMP/htdocs/my-drupal8/web"

<Directory "/Applications/MAMP/htdocs/my-drupal8/web">
        #Options Indexes MultiViews
        Options All
        AllowOverride All
        Order allow,deny
        Allow from all
</Directory>
```

If you clone or download a completed theme directly from this repo, then follow these installation instructions:

##### 1. Install Bootstrap Barrio to enable Bootstrap 4

Run `composer require 'drupal/bootstrap_barrio:^4.22'` command in the root folder of the project.

##### 2. Clone this repo to `[your-drupal]/web/themes/custom`

##### 3. Activate both Bootstrap Barrio and this theme in `/admin/appearance`

Gleb theme should be set as default theme

### To compile SCSS to CSS

##### 1. Get Node.js https://nodejs.org/

##### 2. Go to theme folder and run `npm install`

##### 3. Compile SASS using `node_modules/gulp/bin/gulp.js`