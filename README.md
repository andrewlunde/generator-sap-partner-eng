# generator-sap-partner-eng [![NPM version][npm-image]][npm-url] [![Build Status][travis-image]][travis-url] [![Dependency Status][daviddm-image]][daviddm-url]
> SAP A-Team MTA Base Project

## Installation

First, install [Yeoman](http://yeoman.io) and generator-sap-partner-eng using [npm](https://www.npmjs.com/) (we assume you have pre-installed [node.js](https://nodejs.org/)).

```bash
npm install -g yo
npm install -g generator-sap-partner-eng
```

Create additional subgenerators (For Andrew Only)
```bash
yo generator:subgenerator module-php
```

Then generate your new project:

```bash
yo sap-partner-eng
```

Then (optionally) subgenerate additional modules:

```bash
yo sap-partner-eng:jenkins       ; echo "Add Jenkins(Piper) support"
yo sap-partner-eng:deploy2xsa    : echo "Add Deploy to XSA extension"
yo sap-partner-eng:db-hdb        ; echo "HANA HDB-styled HDI DB"
yo sap-partner-eng:db-cap        ; echo "HANA CAP-styled HDI DB"
yo sap-partner-eng:db-ss         ; echo "HANA SecureStore"
yo sap-partner-eng:module-nodejs ; echo "New NodeJS Module"
yo sap-partner-eng:module-java   ; echo "New Java Module"
yo sap-partner-eng:module-python ; echo "New Python Module"
yo sap-partner-eng:module-docker ; echo "New Docker Module"
```

If you git clone this repo, get it to show up in Yeoman by using npm link from the repo directory. (sudo if perm issues)
```
npm link
sudo npm link
```
The last line of the output should look like this.
```
/usr/local/lib/node_modules/generator-sap-partner-eng -> /Users/i830671/git/generator-sap-partner-eng
```

Yeoman looks for generators installed in:
```
cd /usr/local/lib/node_modules/
```

In SAP Business Application Studio Dev Space:
```
~/.node_modules_global/lib/node_modules/
```

Now when you run yo, you should see a choice called __Sap A Team Mta Base__

For SAP Application Studio (Beta).  Open a new terminal.
```
cd ~
mkdir generators
cd generators
git clone https://github.com/alundesap/generator-sap-partner-eng.git
npm install -g generator-sap-partner-eng
cd ~
cd projects
```

Then generate your new project:


## Getting To Know Yeoman

 * Yeoman has a heart of gold.
 * Yeoman is a person with feelings and opinions, but is very easy to work with.
 * Yeoman can be too opinionated at times but is easily convinced not to be.
 * Feel free to [learn more about Yeoman](http://yeoman.io/).

## License

MIT © [Andrew Lunde](https://github.com/alundesap)


[npm-image]: https://badge.fury.io/js/generator-sap-partner-eng.svg
[npm-url]: https://npmjs.org/package/generator-sap-partner-eng
[travis-image]: https://travis-ci.com/alundesap/generator-sap-partner-eng.svg?branch=master
[travis-url]: https://travis-ci.com/alundesap/generator-sap-partner-eng
[daviddm-image]: https://david-dm.org/alundesap/generator-sap-partner-eng.svg?theme=shields.io
[daviddm-url]: https://david-dm.org/alundesap/generator-sap-partner-eng
