---
layout: post
title: "The Switch to Netbeans"
date: 2014-01-28 00:00:00
categories: abyss blog
---

I mentioned in my first post that I would be developing Abyss Studio on the IntelliJ IDEA platform. Well, that is now
going to change. Don't get me wrong, IntelliJ is probably the best Java IDE around, for writing code. In-fact, I feel
like all of the JetBrains IDEs are superior to other solutions and I have used all of them. I don't want to get
side-tracked and start talking IDEs, so let me explain my reasoning behind abandoning IntelliJ for Abyss Studio.

From this point when I say IntelliJ, I mean as a platform, and when I say Netbeans, I mean the Netbeans Platform. Good?
When I started developing on IntelliJ, everything looked good. I started with some tool windows (sidebars) and they went
together quickly and without a problem. The learning curve wasn't too steep and I was quickly productive. However, when
I started working on the map editor, things got tricky. IntelliJ assumes everything is a source file from the start and
opens all new file types in a text editor. Well, for Abyss map files, we need them to open in a new type of editor
altogether. After hours digging through forums, digging through the IntelliJ source code and beating my head against a
wall, I determined that this is just not going to work out very well. I was eventually able to create a new editor window
and open a dummy map file up. I started to feel a little better until something hit me like a brick. I have to create a
custom project browser, project file type, runtime configuration, etc. Is this doable? I'm sure it is but there is more
to the problem. 

To build against IntelliJ, you have to download the entire IntelliJ source code, develop the custom components as plugins,
test them against an official IntelliJ release, then integrate them into the IntelliJ source code, modify the source code
to remove anything that isn't needed in the custom product, modify the build scripts to account for the changes, rebrand
the application, build the project, run an ant task to create the binaries, then distribute. Sound fun? You bet it isn't!
I was willing to do this, but first I decided to revisit Netbeans one last time. 

I downloaded the latest Beta "8.0", fired it up and started a new Netbeans Platform Application. Then I decided to start
with a prototype of the map editor. With a few button clicks I had the prototype finished. A few other prototypes that
would have been insanely complicated in IntelliJ? A few button clicks did the job again. This is just too easy! What about
all of the cross window communication that has to take place? It is all right there and ready to go! So, for the last 
challenges I decided to figure out how to rebrand the application and package it. In IntelliJ this took place through
various XML files hiding all over the massive project and ant tasks. In Netbeans, I found that I could right click my
project and click "Branding" and a nice window pops up letting me change everything. Then finally another right click
on the project revealed the "Package as..." menu providing options for Windows, zip, Mac app, etc.

Seriously, button clicks allowed me to wireframe, rebrand and package the application in less than thirty minutes!
The choice is a no brainer. I don't want to spend months writing boiler plate code and learning a platform when
another platform can do it in a few nights. I would rather spend the bulk of my time writing code that is relevant
to the engine. I'm sure I will run into some things that leave me scratching my head but I'm feeling really good
about Netbeans these days. It has always been a great IDE and I feel like we will meet great success by trusting
the platform around here.

I know there are people that will disagree with this choice, but ultimately those people need to trust me to know
that I'm making the right decision. If you feel like I'm wrong, then go try out some of the other Corona SDK IDEs
on the market and then come talk to me. Also remember to point me to the ones that support full RPG creation with
graphical tilemapping and all of that fun stuff.

On another note, Jesse got me a couple of tiles to work with today so I can really start getting serious about
writing code. It isn't a lot but it is enough for me to start knocking out the initial algorithms we will be
using to draw maps. That alone should be enough to give you a warm fuzzy feeling. I hope to have some screenshots
to show off by the end of the week so wish me luck!

_Giggles and Chainsaws_

_Dan_