# Synopis 
This is an interactive game on my Pages site.

ParticleZooQuest
============

[ParticleZooQuest](http://particlequest.com/) is a HTML5/JavaScript multiplayer game experiment for making particle physics fun. The goal of this project is to create a science based story modifying BrowserQuest. In order to do so, we are extending the engine, implementing new mechanics and including new graphics.

### Why we do ParticleQuest
ParticleQuest is a project managed by students in their free time and they do it for...
* Learning cutting-edge web technologies.
* Improving their game design skills.
* And enjoying while hacking an awesome videogame! :D

### What we are trying to achieve
After discussing quite a lot what would be the aim, scope and expectations of ParticleQuest, these could summarize the main goals that are planed to be achieved at some point.
* Tell a story about particle physics.
* Complete redesign of the graphics.
* Improve the game mechanics.

### Further and beyond
ParticleQuest was born during a hackathon organized by **Mozilla** at **CERN** and both organizations have shown interest in the project if it happens to come to fruition. That's quite a lot of motivation!


How to get it going
-------------------

ParticleQuest has two major parts:

* the server side, which runs using Node.js
* the client side, which runs in your browser

Getting the server up and running is pretty easy. You need to have the following installed:

* Node.js (**v0.8.x** works, v0.6.x series should work, other versions are unknown - let us know if you test them!)
* gcc-c++ (optional - not needed on windows)
* GNU make (optional - not needed on windows)
* zlib-devel  <-- this is the Fedora/RHEL package name, others may be slightly different.  Not needed on windows.

Clone the git repo:

    $ git clone git://github.com/particlequest/ParticleQuest.git
    $ cd ParticleQuest

Then install the Node.js dependencies by running:

    $ npm install -d

Then start the server by running:

    $ node server/js/main.js

The BrowserQuest server should start, showing output like this:

    $ node server/js/main.js
    This server can be customized by creating a configuration file named: ./server/config_local.json
    [Tues Sep 13 2016 17:16:27 GMT-0400 (EDT)] INFO Starting BrowserQuest game server...
    [Tues Sep 13 2016 17:16:27 GMT-0400 (EDT)] INFO world1 created (capacity: 200 players).
    [Tues Sep 13 2016 17:16:27 GMT-0400 (EDT)] INFO world2 created (capacity: 200 players).
    [Tues Sep 13 2016 17:16:27 GMT-0400 (EDT)] INFO world3 created (capacity: 200 players).
    [Tues Sep 13 2016 17:16:27 GMT-0400 (EDT)] INFO world4 created (capacity: 200 players).
    [Tues Sep 13 2016 17:16:27 GMT-0400 (EDT)] INFO world5 created (capacity: 200 players).
    [Tues Sep 13 2016 17:16:27 GMT-0400 (EDT)] INFO Server (everything) is listening on port 8000

That means its working.  There should not be any warnings or errors.

Using a browser, connect to port 8000 of the server entered above.  The BrowserQuest start page should appear, and the game should work.


Browser Support
---------------

* Firefox (any recent) - Works well.
* Safari 6.x - Background music doesn't play.  Everything else works well.
* Chrome - Sounds effects don't work.
* Chromium - Varies wildly.  Some releases display using BrowserQuest's "mobile" layout, with very small screen.  Not recommended.
* Opera - Doesn't work, no WebSocket support.
* IE (any version) - Untested.


Node.js for Fedora 16 and RHEL6/CentOS
--------------------------------------

On Fedora 16 and RHEL 6/CentOS 6, the rpms here are known to work:

  http://justinclift.fedorapeople.org/nodejs/

Note, those rpms are ugly, unofficial builds by [@justinclift](https://github.com/justinclift).  You are
most welcome to improve on them. :)


Mac OS X
--------

Node installed through Homebrew is known to work. i.e.:

    $ git clone git://github.com/browserquest/ParticleQuest.git
    $ cd BrowserQuest
    $ brew install node
    $ npm install -d
    $ node server/js/main.js

Windows
-------

Windows 8 is known to work ok with just the base Node v0.8.18
installed, without Visual Studio, nor Python, nor the native
extensions for npm modules installed.


Documentation
-------------

Lots of useful info on the [wiki](https://github.com/particlequest/ParticleQuest/wiki).


License
-------

Code is licensed under MPL 2.0. Content is licensed under CC-BY-SA 3.0.
See the LICENSE file for details.


Awards
------
Winner project at [CERN Summer Student Webfest](http://www.citizencyberscience.net/cern-webfest/).

Credits
-------
Originally created by [Little Workshop](http://www.littleworkshop.fr) and continued by [BrowserQuest team](https://github.com/browserquest):
Forked by CERN Summer Students for the [CERN Webfest](http://www.citizencyberscience.net/cern-webfest/).


* Alejandro Avilés - [@OmeGak](http://twitter.com/OmeGak)
* André-Pierre Olivie
* Angelo Marco Ramoso - [@icanseemyhalo](http://twitter.com/icanseemyhalo)
* Jessy Katy Schingler - [@jessykate](http://twitter.com/jessykate)
* Quentin Mazars-Simon - [@quentinms](http://twitter.com/quentinms)

All of the music in BrowserQuest comes from Creative Commons [Attribution 3.0 Unported (CC BY 3.0)](http://creativecommons.org/licenses/by/3.0/) sources.

* [Aaron Krogh](http://soundcloud.com/aaron-anderson-11) - [beach](http://soundcloud.com/aaron-anderson-11/310-world-map-loop)
* [Terrel O'Brien](http://soundcloud.com/gyrowolf) - [boss](http://soundcloud.com/gyrowolf/gyro-scene001-ogg), [cave](http://soundcloud.com/gyrowolf/gyro-dungeon004-ogg), [desert](http://soundcloud.com/gyrowolf/gyro-dungeon003-ogg), [lavaland](http://soundcloud.com/gyrowolf/gyro-scene002-ogg)
* [Dan Tilden](http://www.dantilden.com) - [forest](http://soundcloud.com/freakified/what-dangers-await-campus-map)
* [Joel Day](http://blog.dayjo.org) - [village](http://blog.dayjo.org/?p=335)

Special Thanks!
* mozilla for the original BrowserQuest code
* (Justin Clift)[https://github.com/justinclift] for continuing the original project.
* Franck Lecollinet - [@whatthefranck](http://twitter.com/whatthefranck)
* Guillaume Lecollinet - [@glecollinet](http://twitter.com/glecollinet)

Many other people are contributing through GitHub:

* Myles Recny [@mkrecny](https://github.com/mkrecny)
* Ben Noordhuis [@bnoordhuis](https://github.com/bnoordhuis)
* Taylor Fausak [@tfausak](https://github.com/tfausak)
* William Bowers [@willurd](https://github.com/willurd)
* Steve Gricci [@sgricci](https://github.com/sgricci)
* Dave Eddy [@bahamas10](https://github.com/bahamas10)
* Mathias Bynens [@mathiasbynens](https://github.com/mathiasbynens)
* Rob McCann [@unforeseen](https://github.com/unforeseen)
* Scott Noel-Hemming [@frogstarr78](https://github.com/frogstarr78)
* Kornel Lesiński [@pornel](https://github.com/pornel)
* Korvin Szanto [@KorvinSzanto](https://github.com/KorvinSzanto)
* Jeff Lang [@jeffplang](https://github.com/jeffplang)
* Tom McKay [@thomasmckay](https://github.com/thomasmckay)
* Justin Clift [@justinclift](https://github.com/justinclift)
* Brynn Bateman [@brynnb](https://github.com/brynnb)
* Dylen Rivera [@dylenbrivera](https://github.com/dylenbrivera)
* Mathieu Loiseau [@lzbk](https://github.com/lzbk)
* Jason Culwell [@Mawgamoth](https://github.com/Mawgamoth)

