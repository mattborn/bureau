# Install prerequisites

Use of Terminal in the steps below assumes you are familiar with [bash file + directory operations](http://overapi.com/linux). Try `sudo ` (including a space) before a Terminal command if it complains about permissions + enter your Mac password.

> Warning: By continuing, you agree that I am not responsible if you miraculously break your machine. Nothing here is very complicated, but I am including this disclimer in light of [Murphy’s Law](https://www.google.com/#q=murphy%27s+law).

Use the unabridged documentation links in each section for additional help or to satisfy any curiosities.

## Spectacle

1. [Download Spectacle](http://spectacleapp.com)
2. Drag **Spectacle** to Applications
3. Open Spectacle
4. Make sure **Launch Spectacle at login** is checked
5. Set **Run…** as a background application
6. Close Spectacle
7. Practice using Opt+Cmd+Left, Opt+Cmd+Right, Opt+Cmd+C, Opt+Cmd+F

[Unabridged docs](https://github.com/eczarny/spectacle#user-content-keyboard-shortcuts)

## Sublime Text

1. [Download Sublime Text 3](http://sublimetext.com/3)
2. Open the **.dmg** file + drag **Sublime Text** to Applications
3. Paste `ln -s "/Applications/Sublime Text.app/Contents/SharedSupport/bin/subl" /usr/local/bin`¹ ² in Terminal + press Return
4. Type `subl .` + press Return to open Sublime from the current directory (should see files in Sublime sidebar)

> ¹ As mentioned above, this may require `sudo`

> ² `mkdir /usr/local/bin` if the directory doesn’t exist

[Unabridged docs](http://docs.sublimetext.info/en/latest/index.html)

### Package Control for Sublime

1. Press `Ctrl + `` (backtick) to open the console
2. Paste `import urllib.request,os,hashlib; h = 'eb2297e1a458f27d836c04bb0cbaf282' + 'd0e7a3098092775ccb37ca9d6b2e4b7d'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)` in the console + press Return
3. Restart Sublime

[Unabridged docs](https://packagecontrol.io/installation)

## Oh My Zsh

1. Paste `curl -L https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh | sh` in Terminal + press Return
2. If it asks if you want to install developer tools, click **Agree** and wait until it downloads and installs
3. Restart Terminal
4. Try `mkdir Code && Code` to make sure in installed correctly¹

> ¹ With zsh, you don’t need to use **cd** to change directories

[Unabridged docs](https://github.com/robbyrussell/oh-my-zsh#user-content-getting-started)

## Node + npm

1. Paste `curl https://raw.githubusercontent.com/creationix/nvm/v0.24.0/install.sh | bash` in Terminal + press Return
2. Run `nvm install 0.12` in Terminal
3. Run `nvm alias default stable` in Terminal

Unabridged docs for [installation](https://github.com/creationix/nvm#user-content-installation) + [usage](https://github.com/creationix/nvm#user-content-usage)

## Some node packages

1. Run `npm install -g node-static` to install node-static
2. Run `npm install -g grunt-cli` to install Grunt

Unabridged docs for [node-static](https://github.com/cloudhead/node-static#user-content-node-static) + [Grunt](https://github.com/gruntjs/grunt-cli#user-content-grunt-cli-)

## Github for Mac

1. If you haven’t already, create a [Github account](https://github.com/join)¹
2. [Download Github for Mac](https://mac.github.com)
3. Open Github for Mac
4. Login to your Github account
5. Make sure the name + email¹ is correct since this will be used for all your commits

> ¹ The email you use will be attached to every commit you make. If you are a Gmail user like me, you can add something like `+code` (plus sign followed by anything you want) after the first part of your email address to prevent spam to your primary address. e.g. `your.email+code@gmail.com`

[Unabridged docs](https://mac.github.com/help.html)

## Now what?

Assuming nothing went south, you’re ready to start building things with code. Head back to [Projects](projects.md).