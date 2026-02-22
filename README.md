Roundcube Webmail Skin "Surak"
==============================

A Vulcan-themed skin for Roundcube Webmail. Named after Surak, the father
of Vulcan logic: "Logic is the beginning of wisdom."

The aesthetic evokes a Vulcan Science Academy terminal: clean geometric
lines, burnt orange and steel blue on cool dark surfaces — desert heat
meets cold logic. No scan-lines, no shimmer animations — logic prevails.

Based on the Elastic skin by The Roundcube Dev Team.


INSTALLATION
------------

Copy the skin folder into `skins/Surak` within your Roundcube installation,
then set in `config/config.inc.php`:

```php
$config['skin'] = 'Surak';
$config['skin_logo'] = [
    '[dark]'       => 'skins/Surak/images/logo.svg',
    '[small]'      => 'skins/Surak/images/logo.svg',
    '[small-dark]' => 'skins/Surak/images/logo.svg',
    '*'            => 'skins/Surak/images/logo.svg',
];
```


BUILDING CSS
------------

```bash
npm init -y && npm install less less-plugin-clean-css
npx lessc --clean-css="--s1 --advanced" styles/styles.less styles/styles.min.css
npx lessc --clean-css="--s1 --advanced" styles/print.less styles/print.min.css
npx lessc --clean-css="--s1 --advanced" styles/embed.less styles/embed.min.css
rm -rf node_modules package.json package-lock.json
```


LICENSE
-------

The contents of this folder are subject to the Creative Commons
Attribution-ShareAlike License. It is allowed to copy, distribute,
transmit and to adapt the work by keeping credits to the original
authors in the README.md file.
See http://creativecommons.org/licenses/by-sa/3.0/ for details.
