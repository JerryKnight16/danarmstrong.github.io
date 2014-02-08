---
layout: post
title:  "Interface Blues"
date:   2014-02-08 02:16:00
categories: abyss blog
---

I know it has been a few days since I've posted anything. For that I apologize, sort of.
I don't feel like I should have to post daily, but I do want everyone to stay updated.
I've been slammed at work with release hardening my project there. That is always a fun
time! Aside from that, I've also been taking a bit of time to read through the books I
have that pertain to Abyss. It is amazing how many design mistakes I tend to make when
it comes to Netbeans code. Luckily, taking the time to actually do my homework has proven
useful in allowing me to correct those mistakes. Granted, in some areas, I refuse to
conform and believe that my ideas will provide a better user experience in the end. To
me, the UX is definitely an important aspect.

Jesse has gotten me several preliminary isometric tiles to play with and I have to say
that they are awesome. His skills never cease to amaze me. As I'm wrapping up sprint 1,
I'm getting pretty excited about putting a map together.

What I'm currently working on is writing interfaces. Anyone who has Java experience
knows that this is all about. Basically, wannabe classes that don't do anything.
They just define the structure that must be used by an actual class. Apparently
Netbeans isn't happy with just classes and prefers both interfaces and classes for
communication between modules. Interfaces aren't so bad but it is a bit annoying
since I cannot think of a logical prefix for them. The elements in a project tend
to have pretty generic names... like Object... and Map... More technical readers
will understand why those names are problematic. So it would make sense to name
them something like AbyssObject... or AbyssMap... but then what do I name the
implementation? Many might say "AbyssObjectImpl and AbyssMapImpl!", but that is
not exactly a desireable naming convention to me. If I were writing this in C#,
I would have the answer already, but the last thing I need is the Java patrol
rolling up and burning me at the stake for using C# styles in a Java application.

For now, I'm just sticking with basic names until I can think of something. Except for
that pesky Object interface, clearly I can't call it that. Anyways, the interfaces will
be changing a lot as I go but I want to get the prototypes written so I can have a more
complete idea of what the project file will look like. The current implementation provides

1. Unlimited tilesets
2. Unlimited tilesheets per set
3. Isometric tile mode
4. Unlimited maps
5. Unlimited map layers
6. Any layer can use an image rather than tiles
7. User defined actor sprite size
8. Use BASIC, or FULL character movement sheets

There are a lot of changes that will need to be made before I'm happy but at least the code
is coming along.

I'm also stuck trying to figure out what to do for icons in AS. I don't even know where to
begin when it comes to creating an icon, so I've been scouring the internet looking for
a nice set for a good price. So long as it can be recolored easily, all should be well. At
some point I will recolor the entire application to give it a nice dark theme. I hate nothing
more than staring into blinding, light-colored applications at 2AM.

I believe that about covers what I needed to update everyone on for the night. Until next time

_Skittles and Inch worms_

_Dan_