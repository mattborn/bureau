### Install prerequisites

**Spectacle**

1. [Download Spectacle](http://spectacleapp.com)
2. Drag **Spectacle** to Applications
3. Open Spectacle
4. Make sure **Launch Spectacle at login** is checked
5. Set **Run…** as a background application
6. Close Spectacle
7. Practice using Opt+Cmd+Left, Opt+Cmd+Right, Opt+Cmd+C, Opt+Cmd+F

**Sublime Text**

1. [Download Sublime Text 3](http://sublimetext.com/3)
2. Open the **.dmg** file + drag **Sublime Text** to Applications
3. Enter `ln -s "/Applications/Sublime Text.app/Contents/SharedSupport/bin/subl" /usr/local/bin` in Terminal
4. Enter `subl .` to open Sublime
5. Press Ctrl+` (backtick) to open the console
6. Enter `import urllib.request,os,hashlib; h = 'eb2297e1a458f27d836c04bb0cbaf282' + 'd0e7a3098092775ccb37ca9d6b2e4b7d'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)` in the console to install Package Control

**Oh My Zsh**

1. Enter `curl -L https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh | sh` in Terminal

**Node + npm**

1. Enter `curl https://raw.githubusercontent.com/creationix/nvm/v0.24.0/install.sh | bash` in Terminal

- [nvm](https://github.com/creationix/nvm) including latest stable node + npm
- [node-static](https://github.com/cloudhead/node-static) `npm install -g node-static`
- [Grunt](http://gruntjs.com) `npm install -g grunt-cli`