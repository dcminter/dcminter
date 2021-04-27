# Daveology 101

🙀️ What is this thing called Dave?\
🐧️ Where possible I like to develop under Linux (and have done so since the 0.96c.2 boot/root disk days)\
☕️ I'm a professional Java developer with a zillion years experience in enterprise\
🦀️ Currently I'm learning Rust ... the borrow checker is winning on points\
🇬🇧️ I'm a Brit\
🇸🇪️ But I live and work in Sweden (och jag pratar lite dåligt svenska)\
✉️ I can be contacted by email as dave@paperstack.com\
💰️ From May 2021 I will be looking for work (but [see below](#jobs))\
📜️ For longer writings see [my blog at paperstack.com](https://paperstack.com/)\

## Jobs

From 1st May 2021 **and not before** I will be looking for interesting job opportunities - however I'm quite picky:

  * I'm only interested in *direct contact* from companies - no recruiters please
  * I'm only interested in *small* companies - maximum 50 employees
  * I'm only interested in *product companies* - no consultancies or cost centres thanks
  * I'm only interested in fully-remote *or* Stockholm-based (and prefer some remote even then)

You can find full details of my experience [on my Linked In profile](https://www.linkedin.com/in/dcminter/).

## Java

I enjoy reading [Hacker News](https://news.ycombinator.com), but boy do they have a downer on Java. Meanwhile the ne plus ultra of [blub](http://www.paulgraham.com/avg.html) languages¹ keeps on trucking.

The arguments against it usually boil down to:

  * It's kind of verbose
  * It's not the latest hot and sexy
  * It doesn't have `${feature_du_jour}`

That's then usually rounded off with grudging acceptance that the JVM is alright and maybe a nod to Scala or Lombok. A few half hearted javanauts defend it, and then the circus rolls out of town.

I have to say, it IS kind of verbose, it is NOT the latest hot and sexy, and `${feature_du_jour}` usually turns up just after (or several years/decades after) a new shiny thing is fiercely outshining that.

On the other hand it's rock solid, has vast libraries, and is manageable for terrifyingly large teams. If you want to roll your own startup in three weeks flat you'd be insane to use it. If you want to write a big complicated back-end application that will still be in action twenty years from now without needing 15 consecutive rewrites then you would be a little eccentric not to at least *consider* it.

Anyway, I'm super biased, having been mucking around in Java since the 1.1.x days. I've written books on various libraries and tools and seen Java used to good and bad effect in all sorts of companies. I even messed with Visual J++ once upon a time (but I cleaned my fingernails afterwards).

In the end it's mostly the people that matter. Pick a solid language and don't be too worried what the mayflies call it.

¹*Would it be petty to point out that paulgraham.com currently has an invalid SSL certificate for the domain?*

## Rust

I'm currently getting up to speed on Rust. It's quite the learning curve for someone who's been letting the garbage collector take the strain for over 20 years - and who created his fair share of segfaults before that in 90s era C++. I do not yet fully grok the borrow/lifetime rules, but I'm starting to get the hang of it. There's a similarity between Java's streams+iterators and Rust's iterators that's reassuring though.

So far the best Rust learning text I've found is [Programming Rust](https://www.oreilly.com/library/view/programming-rust-2nd/9781492052586/) from O'Reilly. The copy I have is the 1st edition, but I'll be getting the linked 2nd edition once it's out. I ploughed through the entire thing and had quite a few moments where the "but...?" objections raised in one paragraph were immediately answered in the next one, which is a very nice way to learn.

Good learning links:

  * [A Half Hour to Learn Rust](https://fasterthanli.me/articles/a-half-hour-to-learn-rust) (more a sales-pitch for Rust syntax to developers familiar with other languages)
  * [How to build a Websocket Server with Rust](https://blog.logrocket.com/how-to-build-a-websocket-server-with-rust/)
  * [The Rust Cookbook](https://rust-lang-nursery.github.io/rust-cookbook/about.html)
  * [Rust Container Cheat Sheet](https://docs.google.com/presentation/d/1q-c7UAyrUlM-eZyTo1pd8SZ0qwA_wYxmPZVOQkoDmH4/edit#slide=id.p)
  * [Rust Language Cheat Sheet](https://cheats.rs/) ("sheet" is rather understating it...)
  * [The Rust Performance Book](https://nnethercote.github.io/perf-book/title-page.html)
  * [The Little Book of Rust Macros](https://veykril.github.io/tlborm/introduction.html)

## 3D Printing

I acquired an Ender 3 Pro towards the start of the pandemic and have been creating a few things with it. So far I've found [FreeCAD](https://www.freecadweb.org/) (or at least the version I'm using) to be impossibly buggy; far too many occasions when a modal dialogue with a magic number and no meaningful message pops up. Save often, reload when things get wedged. Instead I've mostly created things with the online [TinkerCAD](https://www.tinkercad.com/) tool - which seems to be far more limited but much more approachable. Next on my list is to learn to use [SolveSpace](https://solvespace.com/index.pl). For the "slicing" step I've been using [Cura](https://ultimaker.com/software/ultimaker-cura) without any problems at all (high praise!)

I've also been playing with strapping a pen to the print head and using it to do plotting. The approach I've used so far is hideous: sending the text through [Scribus](https://www.scribus.net/), [Inkscape](https://inkscape.org/), [a command line SVG to GCode tool](https://github.com/sameer/svg2gcode), a custom bash script to rewrite the GCode to something that works with the lashed-together plotter, and then printing from [Octoprint](https://octoprint.org/). I have a tentative plan to create a CLI tool to go direct from text to GCode. So far my ignorance of TrueType fonts parameters has been the limiting factor!

I also also had to recompile and reinstall [Marlin](https://marlinfw.org/) to allow for a BLTouch (tramming assistant), a faster motherboard, and plotting [G500 Bézier curves](https://marlinfw.org/docs/gcode/G005.html)! That was all rather reminiscent of the early days of PC wrangling when one had the lid open more often than not to get things working!

## Virtual Reality

I've played around a little with [WebXR](https://immersiveweb.dev/) (which used to be "Web VR"), mostly as a tool to get some basic knowledge of WebGL (the only external libraries I used were for the matrix math). Hilariously the WebXR bits were all terribly easy and the WebGL bits (I'd never used even OpenGL before) were terrifically hard! Still, it was fun, and I'd now feel confident picking up [Babylon.js](https://www.babylonjs.com/) or [Three.js](https://threejs.org/) to take that further.

My starting point for learning WebGL was [WebGL Programming Guide: Interactive 3D Graphics Programming with WebGL ](https://www.goodreads.com/en/book/show/16269927-webgl-programming-guide) which is a bit out of date, but not so much that I couldn't follow along. I'm still looking for a good follow-up book but haven't found anything quite suitable for my needs yet.
	
