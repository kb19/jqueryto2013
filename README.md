jqueryto2013
============



<strong>Promises: The Good, The Bad and The Ugly by Dan Heberden</strong
- jQuery’s .deferred implementation of the Promise API
- underscore has a port (?) of .deferred in _.deferred()

<strong>Gone in 60 Seconds by Addy Osmani</strong>
- optimal frame rate for smooth websites → 60Hz
- CSS features like box-shadow / box-radius can have a negative impact on performance by lowering the frame rate and increasing the repaints needed
- lots of tools (some experimental) to troubleshoot site performance in Chrome
    <br>→show paint rectangles
    <br>→show composite layer borders
    <br>→continuous painting mode
- do performance profiling in incognite mode → plugins can affect profiles
- telemetry (?)
- remote debugging in Chrome using ADB + Chrome Dev Tools

<strong>Holy Grail: Javascript on the Client and Server by Tim Branyen</strong>
- Different applications types
    →SPA → TweetDeck
    →ServerSide → GitHub.com
- PhantomJS (headless browser)
- Rendr @ Twitter
- AirBnB post on Render (http://nerds.airbnb.com/weve-launched-our-first-nodejs-app-to-product)
- example of presentation → https://github.com/tbranyen/previewcode.com

<strong>Angular MVW (Model View Whatever) by Pearl Chen</strong>
- Yeoman + Grunt + Bowser (Twitter)
- Angular comes with unit testing integrated
- appliness.com →  digital magazine for web devs
- I think Yelp uses Angular (ng- attributes)
- What goes on under the hood in terms of DOM manipulation and how does it affect performance vs. jQuery?

<strong>Development and Prototyping by Monika Piotrowicz</strong>
- including devs in the design process helps avoid headaches when it comes to implementation
“stagger” approach is BAD → designers may create crazy interactions / ideas and devs have no idea
- @ JetCooper they have ‘pods’ → a dev is paired with a designer for the whole process
- collaborative!
- revisit tools before each project (which have change, what other options are there etc.)
- prototyping helps challenge assumptions, brings up problems early
- bad idea to have designer present client with designers + UX without consulting developer
- JetCooper has demo days where devs showcase what they have been working on
- developer meetings where they just catch up with what they are working on / new stuff / etc.
- “creative recess” → 2 days every month to do mini-hackathons, test new techs, etc.
- when discussing issues with other developers become an ADVOCATE
be CONSTRUCTIVE

<strong>Offline Mobile Wed App Arch + Design by Boaz Sender</strong>
- “traunch” data into separate units instead of trying to pipe it in all at once
- Leafleft.js was most performant on mobile browsers
- Appache → pain to use 
    →define what gets cached
    →appcache-internals → Chrome bookmarklet
- DON’T try to copy native design over to mobile web

<strong>Fixing Broken Windows by Sam Breed</strong>
- book: “The Pragmatic Programmer”
1) Mixed spaces / tabs / trailing whitespace
    →decide on a convention to use!
Have a style guide
jQuery style guide
idiomatic.js
Know your VCS
use pull requests for code reviews
Avoid monolithic files!
leverage the module pattern
Modules
requireJS / AMD
Leave $.fn alone unless you really mean it
Dead code → have a ‘remove commit’ instead
Writing testable code
structure app around ojbect
Don’t retest jQuery
Have a build step! Only ship the code that changes (i.e. not jQuery / big libraries)
Don’t modify native objects with prototype (i.e. String.prototype)
multiple doc readys? NO!
don’t UA sniff
- THINK CRITICALLY!

<strong>Developing with Grunt by Dan Heberden</strong>
- gruntjs.com/plugins → good repo for all sorts of plugins
minimatch?
- Grunt devtools plugin for Chrome
sits in your Dev Tools
- #grunt on Freenode IRC
- you can create a Grunt task to run nodemon

<strong>Front-End Diaspora by Paul Irish</strong>
- use the timeline trace for performance
- new browser feature → requestAutocomplete() → pops up an auto-complete dialog
useful for ecommerce solutions
see the auto-complete input attribute
- see Alex Mccaw’s article on a browser API for one-click checkouts
http://blog.alexmaccaw.com/one-click-signups-and-purchasing 
- checkout OnePassword for password management

Scrolling Performance
- scrolling is important, especially on mobile
root of some mobile vs native debates
- always serve images @ proper size
- -webkit-transofrm = translateZ(0)
paint hack that avoids unnecessarily repainting objects
- Paul Lewis’ article: On Translate3D & Layer Creation Hacks
http://aerotwist.com/blog/on-translate3d-and-layer-creation-hacks/
- checkout the Chrome console doc on Google 

- XCode’s Network Link Conditioner Tool
simulates shitty connections, good ones etc.
- multi-device testing
BrowserStack, DeviceAnywhere
- load http://en.wikipedia.org/wiki/Wikipedia and behold the ‘layout thrashing’ (constant repaints) in the timeline
- chrome://flags → turns on dev tool experiments
- Snippets → cool feature that saves JS snippets
- styled console logs are possible

 Web References<br>
http://aerotwist.com/blog/on-translate3d-and-layer-creation-hacks/<br>
http://blog.alexmaccaw.com/one-click-signups-and-purchasing<br>
http://nerds.airbnb.com/weve-launched-our-first-nodejs-app-to-product<br>
https://github.com/tbranyen/previewcode.com<br>
