Wolph42🐺 — 5/16/2020 9:58 AM

I've been toying with the idea to creata an inn generator in MT, but I once did a full blown solo game generator and that turned out to be more than I could chew, so If I'm to do it I would like to do this as a joint effort.

Basically anyone interested can join the project, you don't have to be a coder. Some dedicated support though would be great:
- mainly looking for enthusiastic people, If you think you cannot attribute with any skill then at least I can presume you can surf the interweb looking for stuff. As I think a LOT of searching will be required. So reallly: anyone who wants, can help/join
- someone who could create 'tiles' (art work) we can use
- other coders obviously
- designers and architects both in terms of HOW would you make this random and how do you generate
probably forgetting other people we might need. But enthusiast are welcome as well. 

To make this somewhat 'doable' as a project  I was thinking to start to 'just' do a common room (as that the most important anyway) and thus leave out other floors like 'bed room' çellars' and other rooms like 'kitchen', 'storage'. 

But first: is anyone interested in working on this with me? 
ok let me start with filling in some ideas, so people get an idea of whats required or shoot at it:
==========================
1. Initially a simple 'room', so random width and height (within boundaries). 
that will be really simple to implement. 
2. place walls, door(s) and windows (again has to make some sense)
3. place floor tiles
4. place bar
5. place hearth (optionally)
6. place tables with chairs (and chairs next to bar)
7. place patrons

To do this I need lots and lots of tokens and they have to be annotated. E.g. we could start with 'fantasy' and 'sci-fi' then e.g. 'table' tokens would be annotated as follows:
"fantasy-poor-6-1" where:
'fantasy' is the setting, can add settings later on like 'scifi'
'poor' bar type: poor, common, good
'6' is the number of seatings
'1' is version of that table e.g. you have 3 versions: 1,2,3 so you get a bit more 'random'. 

The same needs to be done for walls, floors, bar, patrons.

As you can see: coding will be limited (initially) I can pull that off, but creating a full collection of annotated tokens is a LOT of work and thats where hands com in. Preferably they're created by someone but we can use existing stuff, I can probably share a sh#tload of tokens but I need people to help sort and annotate.

In later stage we can also add mugs, candles, lights etc.
Later then that we can add a name generator, description generator and probably an 'event' generator. Add menus etc. Another route is adding rooms, floors, cellars etc. But: common room first.
============================= 
