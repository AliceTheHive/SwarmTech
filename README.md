# SwarmTech

Realtime coordination demo for disaster response teams.

# Contributing

To begin contributing, please fork the repository to your personal account, clone it, and submit a pull request.  We'll respond with comments and should have your patch merged in short order.  If there are any problems with this process, please talk to us on [gitter.im/JSVillage](https://gitter.im/JSVillage).

# Running the project for developers/testers

Basically all we need to do is serve a static site.  If you alreaady know how to do that, feel free to serve the root directory of this project.  Otherwise, keep reading to set up a simple Node.js server.

Open a terminal on Mac or Linux and enter the following commands.  On Windows?  Get [git](https://git-scm.com/downloads) first, then run `git-bash` and do the same.

```
# install nvm
curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.8/install.sh | bash

# check for latest version of node
nvm ls-remote

# install, for instance node.js v8.6.0
nvm install v8.6.0

# install static webserver to serve any directory you want
npm i -g node-static
```

Now we can serve the site:

```
cd [where-ever-you-cloned-this-repo]
static .
```

Then just open your browser at [http://127.0.0.1:8080](http://127.0.0.1:8080).

You'll have to refresh the page any time you make changes to the code, but other than that it's not bad.  If you want livereload, [someone's made a project for that](https://github.com/farf/static-livereload), but it's a little bit more cumbersome to configure.  Maybe someone could fork [node-static](https://github.com/cloudhead/node-static) and add livereload?  If you do, feel free to update this documentation with your wonderful improvements.  :-)

# Making Changes

Well, it's just good ol' HTML, CSS, and Javascript.  You were expecting a build process?  Sorry.  We're too lazy for that (and it serves as an unnecessary barrier to learning).  We do use vue.js, so it should be possible to keep this code somewhat modular and well kept.

Take a look around and edit files as you see fit, then refresh to see your changes.  May the force be with you!