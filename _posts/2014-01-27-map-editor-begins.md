---
layout: post
title:  "Map Editor Begins"
date:   2014-01-27 02:30:00
categories: abyss blog
---

Just a quick update to cover the day. Most of my day was spent working on the site here and getting it ready
to go. I played around with UserVoice a bit and then added AddThis. Sadly, on mobile devices, they do not
work together because the AddThis "share" menu covers the UserVoice button. This irritated me but I eventually
decided that the ability for you guys to share posts is more important than a contact form. At least that is
true for the time being. In the long run, if someone needs to contact me they can always use Disqus or
Github.

Aside from working on the site, I have started putting the map editor together in Abyss Studio. If there is
one major downfall to using IntelliJ as my foundation, it is the complication found in creating a custom
editor window. Tool windows take about 20 minutes to design, develop, test and deploy. Editor windows on the
other hand require significantly more work. The map editor itself should go together pretty quick once I 
get the window and all required components figured out. Luckily, I do have the IntelliJ source code
available and it contains a semi-relevant component that I'm able to use as a reference.

So far I have the tileset window, map properties window and map layers windows mostly completed. I will just
have to go back once the map editor window is finished and start tying them all together. The code is dirty
at the moment, but that's how it works most of the time. This is all proof-of-concept code and is subject
to significant changes as I put all the pieces of this puzzle together.

My biggest hurdle right now is the format to store the maps in. In my first pass I've been keeping them
as native Lua tables. This has the benefit of offering amazing speed, but it takes more disk space
and it is more difficult to parse in the editor. I have considered storing them as JSON objects, which
takes just as much disk space, is slower to load but easier for Java to parse. Corona provides native
JSON parsers, so this may be idea. I'm also debating on a custom binary format to store the maps. This
provides the smallest size but does require a parser to be written in both Lua and Java. While the 
parser would probably be simple enough depending on the final result, that does eliminate the possibility
of a game developer being able to edit the file with a text editor. While that is a non-issue, it does
bug me a bit.

I will most likely go with JSON when it is all said and done. If they start taking too much space then
custom format it is. If anyone has any input concerning this matter then don't hesitate to voice your
opinion.

_Hugs and Butterflies_

_Dan_