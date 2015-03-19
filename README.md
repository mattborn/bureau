# bureau

A few dozen things every front end developer should know.

> Knowing your options is proficiency. Limiting your options is mastery.

## Local environment

### Machine

Be familiar with [Linux](https://kali.org) + [Windows](https://github.com/xdissent/ievms).

Use a [Macbook](http://store.apple.com/us-hed/buy-mac/macbook).

### Window management

Be familiar with [Divvy](http://mizage.com/divvy), [WindowTidy](http://lightpillar.com/macos/windowtidy), [Spaces and Mission Control](https://support.apple.com/kb/PH18809).

Use [Spectacle](http://spectacleapp.com).

### Browser

Be familiar with [Firefox](https://mozilla.org/en-US/firefox), [Safari](https://apple.com/safari), [IE](https://windows.microsoft.com/en-us/internet-explorer), [Opera](http://opera.com), [Mozilla](https://mozilla.org), [webkit](https://webkit.org), and [blink](http://chromium.org/blink).

Use [Chrome](https://google.com/chrome) or [Canary](https://google.com/chrome/browser/canary.html).

### Code editor

Be familiar with [nano](http://nano-editor.org), [emacs](http://gnu.org/software/emacs), [vim](http://openvim.com), [Dreamweaver](http://dreamweaver.com), [Coda](https://panic.com/coda), [Atom](https://atom.io), and [Brackets](http://brackets.io).

Use [Sublime Text](http://sublimetext.com).

### Command line

Be familiar with [bash](http://overapi.com/linux), [zsh](http://zsh.sourceforge.net), and [Terminal][terminal].

[terminal]: http://en.wikipedia.org/wiki/Terminal_(OS_X)

Use [Oh My Zsh](https://github.com/robbyrussell/oh-my-zsh).

### Interpreter

Review the following:

Compare | Javascript | PHP | Ruby
--- | --- | --- | ---
Dependency management | [npm](https://npmjs.com) | [Composer](https://getcomposer.org) | [gem](https://rubygems.org) + [bundler](http://bundler.io)
Build tool | [Grunt](http://gruntjs.com) | [Robo](http://robo.li) | [Rake](https://github.com/ruby/rake)
Static site generator | [Assemble](http://assemble.io) | [Sculpin](https://sculpin.io) | [Jekyll](http://jekyllrb.com)
Framework | [Meteor](https://meteor.com) | [Laravel](http://laravel.com) | [Rails](http://rubyonrails.org)
Microframework | [Express](http://expressjs.com) | [Slim](http://slimframework.com) | [Sinatra](http://sinatrarb.com)
Templating | [Handlebars](http://handlebarsjs.com) | [Twig](http://twig.sensiolabs.org) | erb + [Haml](http://haml.info)

Also, [compare languages side-by-side](http://hyperpolyglot.org/scripting).

**TL;DR:** Javascript is the only *isomorphic* web language meaning we can use it on the server + the client. The decision is easy: we learn, live + love Javascript.

Be familiar with [Node](https://nodejs.org), its [REPL](https://nodejs.org/api/repl.html), [ECMAScript 5](http://kangax.github.io/compat-table/es5), [Harmony (ES6)](http://kangax.github.io/compat-table/es6), and [npm](https://npmjs.com).

Use [nvm](https://github.com/creationix/nvm) to install [Node](https://nodejs.org) + [npm](https://npmjs.com).

### Webserver

Be familiar with [Cactus](http://cactusformac.com), [MAMP](http://mamp.info), [Pow](http://pow.cx), and the [native LAMP stack on OS X](https://urbaninsight.com/2014/09/22/semi-native-lamp-stack-os-x).

Use [node-static](https://github.com/cloudhead/node-static).

### Build tool

Compare | [Grunt](http://gruntjs.com) | [Gulp](http://gulpjs.com) | [Broccoli](http://broccolijs.com) | [Jake](http://jakejs.com)
--- | --- | --- | --- | ---
File | `Gruntfile.js` | `gulpfile.js` | `Brocfile.js` | `Jakefile`

[Read this](https://medium.com/fear-and-coding/grunt-vs-gulp-vs-make-vs-rake-vs-jake-vs-cake-vs-brunch-vs-ant-vs-maven-vs-bash-vs-you-6a149329f050)

### Document stack

Be familiar with [Blacksmith](https://github.com/flatiron/blacksmith), [Wintersmith](http://wintersmith.io), and [Jekyll]().

Use the following:

Layer | Library
--- | ---
Static site generator | [Assemble](http://assemble.io)
Github deployment | [grunt-gh-pages](https://github.com/tschaub/grunt-gh-pages)

### Application stack

Be familiar with [jQuery](), [Zepto](), [Underscore](), [Angular](), [Ember](), [Meteor](), and [Backbone]().

Use the following:

Layer | Library
--- | ---
View | [React](http://facebook.github.io/react)

## Remote environment

Be familiar with [bash](http://overapi.com/linux), [ssh (basic syntax)](https://digitalocean.com/community/tutorials/how-to-use-ssh-to-connect-to-a-remote-server-in-ubuntu), [rsync](http://en.wikipedia.org/wiki/Rsync), and [Apache](http://httpd.apache.org).

Use [nginx](http://nginx.org) + [Express](http://expressjs.com).

### Free hosting

[Github pages](https://pages.github.com)

### Paid hosting

[DigitalOcean](https://digitalocean.com) + [dokku](https://github.com/progrium/dokku)

## Proficiency path

Make sure you have the following installed:

- [Spectacle](http://spectacleapp.com)
- [Sublime Text](http://sublimetext.com) including `subl` command
- [Oh My Zsh](https://github.com/robbyrussell/oh-my-zsh)
- [nvm](https://github.com/creationix/nvm) including latest stable node + npm
- [node-static](https://github.com/cloudhead/node-static) `npm install -g node-static`
- [Grunt](http://gruntjs.com) `npm install -g grunt-cli`

### New repo in Github

![](https://dl.dropboxusercontent.com/s/zw0us7hkw7ipr3s/github-new-repo.png)

```
~/Code && git clone git@github.com:mattborn/bureau.git && bureau
```
*Note: `~/Code` should be wherever you keep all your repos. Also, this step is an example + you should be creating a new repo since this one will already include all the upcoming steps (unless that’s what you want).*

### Initialize as node project

`npm init`, then just keep hitting Enter for all the questions since you can always change this stuff later in your `package.json` file if it starts to matter.

### Install dependencies

```
npm install --save-dev assemble grunt grunt-gh-pages
```

### Directory structure

`mkdir src && mkdir src/partials && mkdir src/pages && mkdir src/posts`