---
layout: post
title:  "Welcome to the Abyss"
date:   2014-01-26 02:00:00
categories: abyss blog
---

The Story
---------
Welcome to the Abyss development blog. I would like to take a few moments and tell you how this all came about. To start with, my name is Dan
and I'm the lead developer of Abyss. I'm a software engineer at the largest tech company in the world and for several years I have been working on enterprise
cloud applications. I enjoy that work but I always like trying new things as well. Recently I met one of the most awesome guys I have ever met who asked
me a question I had not been asked before "Have you ever done any game development?" Well, no, I never had. He proceeded to tell me about a game he is
developing (more on that later) and it started to capture my interest. When I got home that day I started looking at various game engines and trying things
here and there but I wasn't happy with anything I found; I'm not an artist, I'm a developer. 

Unity is amazing but too complicated since I have absolutely no skills in 3D modeling. GameSalad is too... well... GameSalad. Construct 2 is very nice, but 
again, not really for a developer. Then I came across an old classic, RPG Maker. I could write 'some' code, it was easy, and it has a ton of resources available. 
I set out to make an RPG for my wife and soon found myself getting pretty mad at RPG Maker. So many things in the editor just didn't make sense and there 
were too many limitations. After a couple of weeks I couldn't handle RPG Maker anymore. I decided to continue my search for a suitable engine. I never found 
an engine I liked but I did find an SDK I liked. 

I had found the [Corona SDK][corona]. At first I was skeptical of what it might offer, but I quickly discovered that it had great potential. The only downfall 
was the fact that my RPG Maker assets were in no form or fashion suitable for it. And it doesn't really have any true tiling abilities out of the box. Call
me old fashion but I like tiles. I set my RPG ambitions aside for a few days and developed a really simple game for my son (he's only 19 months old). It
was very nice working with Corona since everything was coded in Lua and the API is incredibly simple. But I still had an RPG in the back of my mind.

During all this time, I'm working on a massive project at work and as part of that project, I'm responsible for creating a custom IDE. I have created entire
IDEs from scratch before, but this time I decided that it would be best to use an existing platform as my foundation. I started messing around with the Netbeans
platform and the Eclipse platform and almost settled on Netbeans when something caught my attention. I use many development tools in my work and
for this latest project (written in Node.js) I had recently purchased a copy of WebStorm by [JetBrains][jetbrains] (the makers of IntelliJ IDEA). I have
become a huge fan of JetBrains' products and I decided to check into whether or not they provide a platform for developing IDEs. As it would turn out, they
do. While not as simple as the NetBeans platform, I find it significantly more powerful but before I commited my team to developing on the IntelliJ platform I 
decided I needed to work with it a bit first.

So, at the end of all of this I have made several decisions. I want to make an RPG and I want to use RPG Maker resources because I'm terrible at graphics.
I want it to be on mobile platforms because I want to learn more about the mobile space. I need to get familiar with the IntelliJ IDEA platform. So I started 
writing code with the Corona SDK to draw maps using RPG Maker VX Ace resources and soon found it to be working very well. Next I started writing plugins for 
IntelliJ to handle drawing tilesets and the likes and found that to be very successful. I decided that the next logical step was to develop an entire RPG
engine and studio to make my game. I started planning the features that I cared about and figuring out what my goals were. Since I am a huge fan of
open source, I decided that I have to give back to the community. But that led to a slight problem; I didn't have any graphics that I could give away
with the engine.

I'm always a bit hesitant to discuss a project I'm working on before I have it ready to show, but I knew I that I had to have graphics for this engine.
When I started playing with RPG Maker, the most amazing resource packs I found all had one thing in common; they were made by one guy over at 
[Pioneer Valley Games][pvg]. I figured that if I was going to distribute graphics with my engine, that I had to approach Jesse and see if he would be
willing to make them. I fired off an email describing my plans and it wasn't long before he was on board. What I found out was that Jesse isn't only
an awesome artist, but he is also very insightful when it comes to desireable game engines. As a guy who has tried them all and kept up with all
of the shortcomings, he has already proven extremely helpful in building my roadmap. We are still early in our discussions, but he has consistently
made suggestions that I hadn't even considered. My goals were to basically make an improved version of RPG Maker that exported games for mobile platforms
and that was compatible with RPG Maker resources. What is happening is that I'm developing an RPG engine that may very well take the indie RPG scene
by surprise.

Last but not least, I said I would get back to the guy who was responsible for all of this. Ryan Green is an indie game developer who is working on
a very ambitious project. He is also the father of four, including a four year-old who has terminal cancer. His project is an amazing game called
[That Dragon Cancer][tdc] that tells the story of their battle with cancer. I have known Ryan for a short time, but he is one of those guys that
never really feels like a stranger. He has a huge heart and he just projects love all around him. His game is slated to be released on Ouya this
year but I know that development costs are not cheap by any means. And I cannot even begin to imagine the medical expenses he is suffering with
Joel's treatments. I've decided that while my game engine and tools will be open-source, that I will charge a small fee for binary copies of the
IDE and donate those proceeds to Ryan and his family. 

I don't want it to ever appear that I'm out to get rich on this project because that is definitely not the case. I just want to make an RPG. As a
result, I am making my own game engine and providing my sources to the community. Part of that involves bringing Jesse on board and making my engine
something that he can use to make his games as well. Since none of this would have happened without Ryan asking a very simple question, I figure
I might as well use this project to help him out a little as well. I will say that I plan to charge significantly less for this engine than
any of the other commercial tools out there that are less powerful than what we are working on. I do not believe in releasing half-baked software
and I believe that even people with limited funds deserve access to professional quality tools. At any rate, all of the source code will be
available under the Apache 2.0 license so those who can't purchase a binary are always free to build it themselves.

That went on a little longer than I had anticipated but I felt like some background was required. Now, moving on to what we are working on!
The RPG I'm writing is being written specifically for my wife, and being such, I'm not going to give away the storyline yet. All I can say
is that it is a deeply psychological game and it is rather dark. It also contains many Christian elements as our faith plays a big part in
our lives (don't worry, I'm not here to push my beliefs on anyone). In planning the game, my wife and I had many discussions about what she
did and didn't like in various games and I took notes along the way. I also took notes about what I did and didn't like about RPG Maker.
Lastly, I read Jesse's wishlist and made a lot of decisions based on his input as well. In the end, here is what we have lined up:

Part 1 - The Abyss Engine
-------------------------

The engine will be a plug and play library for the CoronaSDK providing many features that require questionable scripts in RPG Maker.

1. Unlimited map layers
2. Unlimited tile sheets
3. Side-view and ABS battle systems
4. Awesome windowing system
5. Configurable tile size
6. Isometric map support
7. True scene management
8. True cutscene support
9. HUD components and API
10. Event & Object differentiation
11. Full frame movements
12. Compatible with RPG Maker auto-tiles
13. Hi-res graphics!
14. Ready to use graphic assets by Pioneer Valley Games!
15. Much, much more!

Part 2 - Abyss Studio
---------------------

The pride and joy of this project will be the studio. This is the graphical tool where all the game making will happen.

1. Built on top of the incredible IntelliJ IDEA 13 platform
2. Quickly add map layers and tile sheets
3. Map layers can contain tiles or images (with configurable opacity)
4. Excellent actor, event, object, etc. management
5. Full featured source code editor
6. Integrated debugging
7. Gorgeous interface!
8. Much, much more!

Currently, I'm still in the planning and experimenting phase of the project but don't let that dissuade you. I'm no stranger to massive
projects and I have the skills and expertise to see this through. All source code will be hosted on GitHub as I go and I welcome the
community to get involved and help out with code, or ideas, or music, or anything they want to contribute. I will go ahead and end
this post since it is too long and too late but be sure to keep checking back as I will keep this blog updated with news and code
samples and all of that good stuff as I go.

_Wiggles and Rainbows_

_Dan_

[corona]: http://coronalabs.com/products/corona-sdk/
[jetbrains]: http://jetbrains.com
[pvg]: http://pioneervalleygames.com
[tdc]: http://thatdragoncancer.com
