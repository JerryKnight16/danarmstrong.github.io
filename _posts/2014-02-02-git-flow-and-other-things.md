---
layout: post
title:  "Git Flow and Other Things"
date:   2014-02-02 02:00:00
categories: abyss blog
---

If you have been looking at the Abyss Studio repository and noticed that no
commits have happened, then I am glad to correct you. I commit at least
once a day. I'm a fan of the git flow branching strategy and I have
adopted it into this project. Right now I'm working on the "New Project"
feature branch. Once I complete that feature, it will be merged into
the develop branch. The master branch won't see activity again until
a stable release is ready. Explaining git flow is beyond the scope
of my blog but you can read all about it at [Git Flow][gitflow]. All you
really need to know is that I'm working diligently and pushing code daily.

On the other front, I got my hands on a copy of a very handy book today.
Since it looks like Netbeans is going to be my platform of choice for
a while, I figured I should go ahead and get some documentation on it
beyond what Google has to offer; surprisingly, good documentation on
the platform is lacking in a lot of areas. So, I grabbed a copy of
_The Definitive Guide to Netbeans Platform 7_. It is proving very useful
so far and I feel like it was a very justifiable purchase. Hopefully
it helps speed development along as I hammer out code.

I'm currently working on the "New Project" and "Save Project" user stories.
These are quite important to moving into creating and editing maps. As a
prerequisite to that I needed to be able to set the "project home" directory
so that I had a default location to store newly created projects. I was
able to implement that tonight. This resulted in a singleton to manage
configuration data, a window to set the data and all other relevant bits.
Just to get it out of the way, I added OS detection and the components to
set the Corona SDK path. A bit more work is required to validate the Corona
path but I can touch that up when I get to the corona features.

Aside from that, I have also started building the new project wizard. This
is actually turning out to be relatively simple, but there is still a bit of
learning required to understand how to make the wizard behave exactly how I 
want. Mostly in the tree views I'm using in the wizard. I anticipate it to
be ready in the next day or so.

To end this, I will share a couple of ideas I've had with the Abyss DevKit.
I'm building the wizard to be relatively agnostic to the platform so that
I can potentially provide support for more than just Corona in the future.
I would like to see the engine be able to export to Mobile, Web and PC
(Mac/Win/Linux) when all is said and done. As a result, I'm writing the
ability to support this into Abyss Studio from the start. 

As far as DevKit versioning goes, I have decided that the best way to go about 
updating the engine libraries is using Git directly. Since NetBeans provides a
Git library, it shouldn't be to hard to just "fetch" the latest version from 
GitHub periodically so that you guys are always up-to-date. That is still  a ways 
out but my brain is always thinking ahead so that I'm not stuck scratching my 
head in the end.

So, that is all I have for tonight. I will update you all again when I have
more news for you.

_Sharks and High Fives_

_Dan_

[gitflow]: http://nvie.com/posts/a-successful-git-branching-model/
