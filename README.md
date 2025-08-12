# spooler

<img width="400" alt="Screenshot 2025-06-13 at 13 56 24" src="https://github.com/user-attachments/assets/52db9688-6b4d-4a57-bc05-dc3706609a33" />

A film bulk loader for up to 30m of film.

[Here's a link to Fusion 360 project in the cloud.](https://a360.co/4kNz4AA)

[Here's a link to Makerworld page](TODO: ADD A LINK)

> This work is licensed under the **** (TODO: pick one) license. This means that you are free to download and print it for your non-commercial use-cases. Any improvements and modifications have to credit the original work and have to be made available under the same license. This is to ensure that everyone can benefit from other people making the design better in the future. It does not allow commercial use.

------


**Who is this document for and how to read it?**

This document is supposed to offer enough detail for people who want the "marketing pitch" as well as thinkerers and makers.
It contains sections that explain the function of the _spooler_ but it also explains why it was designed that way.
Additionally, sometimes it contains special notes for people that might want to tweak certain parts or aspects to optimize the design for their specific printers and the materials they use. This might be relevant if you are printing with a filament with a very different properties (like expansion) than me (I am using PETG made by [Plasty Mladeč](https://www.filament-pm.cz)) as there are certain parts that require at least a modest amount of care to fit properly. I do believe it shouldn't be an issue as I have built in quite enough tolerance into the design already, but I will point out the pieces and their bits where you might want to pay at least a little bit of attention.

If you have a lot of experience with 3D printing and bulk loading, I believe you should be able to just quickly scan the document and extract the bits relevant to you before you start printing.


## Features and Design Decisions
Here are the main design goals and corresponding features of the spooler. The spooler is by no means perfect or absolutely fool-proof or rather—it does not reach the level of polish I imagine from a commercial solution, operating it requires a little bit of dexterity still.
However, I believe it is a step in the right direction and since I am open-sourcing it someone might be able to modify the design and make it even better. One of my key rules was to never compromise the main bulk-roll compartment in any way. There are no holes for screws or anything else that would go directly into the bulk-roll compartment. This should give you confidence that the _spooler_ will manage to keep your film in the dark, once the bulk roll is loaded.

Here are the key features that make the _spooler_ stand out.

### Ease of Use
My goal was to make a bulk film loader that would allow an easy manipulation with the film cartridge. I wanted to have the space where the film canister goes as open and accessible as possible. The _spooler_ achieves this by the film canister space being open from the front and top and mostly open from the sides. More details about how to operate the "door-mechanism" in the section on how to operate the spooler.

### Modularity
There are different film producers and they might use differently shaped and sized spools. The film canisters are also little bit different. The canister cores from different manufacturers (the little bit that you twist and roll the film around, or rather your camera does that) have small variations in diameters. This is why the _spooler_ has those two bits interchangeable.

These two interchangeable parts use magnets to keep them in place. It's quite useful to have the cartridge holder kept in place by magnets—you don't have to deal with it moving and getting misplaced when manipulating the film cartridge in the loading-space.

The interchangeable rod that holds the bulk spool has another feature. Because it spins together with the bulk roll of film, the film does not spin on the inside of the spooler and there should be no unnecessary friction. It is also designed to raise the bulk roll a little from the bottom of the _spooler_ so that the film's edges don't touch the floor. _This is hard to verify as I can not see inside the spooler._

There are files for the spool rod that fits bulk cores from Foma. I don't have access to bulk rolls from Illford or Kodak. Anyone is free and encouraged to either submit the right dimension for other spools or design it and push it into the repository.

### The Lever
The lever used for twisting the film into the cartridge does not need to be held or pushed down for it to stay in place. This way you don't have to worry about accidentally exposing the inside of the loading space in the middle of the process. The key-shaped lever is held in place by friction inside the "door-mechanism". You can learn more about this in the section on operating the spooler. This makes using the key-shaped lever pretty comfortable.


### Film Indicator
When you get to the end of the bulk roll it is very easy to wind the end of the film all the way into the film cartridge without noticing. To prevent this, the _spooler_ has a special feature in the center of the lid. There is a circular cavity made for a small magnetic ball bearing to go around. The rod that goes into the bulk roll (or rather the bulk roll goes into it) has a cavity to fit a strong cylindrical magnet. The position of the magnet makes it so that when the rod spins, it moves the ball bearing. When you can see the ball moving (or hear it), you know there's still film attached to the core of the bulk roll. Once the ball stops going around, you know the bulk roll is done.
This solution allows you to know when you run out and carefully gauge how many turns you want to make before opening the door compartment to "catch the end of the roll". This specific design works without compromising the bulk-roll compartment.




## How to Print it
I have published print profiles for users of Bambu printers. You can find them here (TODO: add the link).

Users of other printers can download the `step` files and print the parts either using my settings (TODO: add a link to a file with settings and explanations of those) or their own settings should they decide to make adjustments.

I recommend printing it with a black filament for maximizing the light-sealing property of the tool.

I print each light-critical part with at least 5 layers for walls. This means that there are usually at least 10 layers between the outside and the inside of the light-sealed compartments. In my experience, this is enough to prevent light from seeping through.

> If you need help with printing, you can [open an issue](https://github.com/jalivert/spooler/issues/new/choose) and I will try to help.

### Printing the Lid with a Ball Magnet In-place
The only somewhat tricky part is the lid of the _spooler_. The lid has a small "tunnel" cavity in the center for the ball-shaped magnet. It is designed so that the ball can not exit the cavity (so that you can't lose it). Because of that, it has to be inserted during the printing process. In short, you have to insert it before the 22nd layer of the lid is printed as that layer goes over the tunnel. For obvious safety reasons, the "official instructions" are: pause the print shortly to make sure that your hands do not interfere with the printer head. The plate is magnetic so that will make it easier for the ball to stay where it should.

> PRO TIP: I recommend having a larger magnet nearby in case you drop the ball in the wrong place so that you can quickly retrieve it.

The "floor" of the tunnel (from the ball's perspective) has to be as smooth as possible. For that reason, I have added a modifier and also changed the settings for the seam (so that it's not aligned as that would case a narrowing in the tunnel at one spot and prevent the ball from moving freely). If there are any issues and the ball is not spinning freely once the lid is done printing, you might need to investigate what is going on.




## How to Assemble it
One key part of the assembly is gluing enough felt in various places. This section will walk you through it and offer explanation of why the felt is important for both light sealing and correct function. Another key aspect is how the lid is attached to the body of the spooler. To take care of that, you will need some extra material and tools. Finally, all the modular parts as well as the "empty bulk" indicator use magnets. I, personally, use neodymium magnets.

### What You Need Aside from the 3D Printed Parts
The lid and the body are held together using 7 M3 heat inserts and screws. You will need to buy those.
It seems possible to instead tape the lid and the body together with a black electrical tape. For that, you will need to print the alternative lid with no holes. It should not be necessary, but it's better to be safe than sorry.
If you decide to use the heat inserts, you will need something to heat them with and push them into the body of the spooler.

So here's a list of things you will need:
- [X] **7 pieces** of M3 heat inserts (I use the short version)
- [X] **7 pieces** of M3x10 screws
- [ ] 4 mm ball-shaped magnet
- [ ] **2 pieces** of 3 mm x 3 mm cylidrical magnet (diameter x height)
- [ ] 8 mm x 10 mm cylidrical magnet (diameter x height)
- [ ] **2 pieces** of 5 mm x 1 mm cylidrical magnet (diameter x height)

- [ ] superglue
- [ ] some black felt (cca 1 mm thick)
- [ ] soldering iron/pen (for heating and inserting)
- [ ] M3 bit


### Inserting the Threads
You will need to use the soldering iron/pen to heat the insert and push it into the hole. I give it a moment to heat up before I start gently pusing. You should not need to fight the material and you should push gently and slowly to make sure the thread is in straight and not too deep.

> PRO TIP: If you ever need to dispose of the _spooler_ and would like to re-use the threads, you can prepare the correct screw and use the soldering pen to heat the insert and then quickly pull it out using the screw. It should take just a moment of heating and not a lot of force. You want to use just the right amount of heat so that the insert comes out clean without excess plastic. (You should be able to pull the thread out completely clean.)

### Gluing in the Felt
There are a few different places where you should apply the felt.

#### Felt in the Narrow Passage of the Body
You need to apply the felt into the narrow passage in the body of the _spooler_. This felt serves a light-sealing purpose so you want to cut it just right. I like to measure the right height (from the floor to the edge of the walls) and make it twice as long than what I need. I then fold it in half and insert it into the narrow passage between the two walls all without applying any glue. I make sure the felt is in place and nicely straightened out. Only then I apply a small amount of glue in a vertical line to attach the felt's end (each) to the wall. There is no need to apply the glue anywhere else beside the ends of the felt. This way you just apply the glue four times and push gently onto the felt and hold it for a couple of seconds.

#### Felt on the Inside of the Door
The whole inside of the door needs to be covered in felt as well. I like to cut the height a little bit longer so that I can wrap the felt over the bottom edge of the door and glue it there too. It makes it a really nice to use (no edges). Again, I only apply the glue locally in small bits all around the edges of the felt. This felt serves two purposes. It fills in the gap between the sliding door and the body of the _spooler_. It also creates enough friction for the turn-key to fit snugly and stay in place. They disc of the turn-key is designed with the felt in mind, so you have to put it all the way up otherwise there's going to be a gap and it won't have enough friction to stay in place. Also, it just looks nice with the entire inside of the door padded with black felt.

#### Felt on the Top of the Lid
There's one more place where a little bit of felt needs to be applied. The placement of this felt ensures that there is no light comming into the loading compartment from the top. You can start by cutting a rectangular felt large enough to go from left to right and then cut it strategically so that you can fold it over the edge and glue it there too. Once again, the disc of the turn-key is designed with this felt in mind, without it, there might be a small gap that might let in light.


### Gluing in the Magnets
Gluing in the magnets should be an easy job. They should fit nicely in the holes with not a lot of force necessary. It should also take just a tiny bit of glue per magnet/hole.

You should make sure to not over-push the magnets too deep in the hole. (The holes are a tiny bit larger to accomodate for the material expansion.) To maximize their effect, they should be touching when the modular part is in place.

> PRO TIP: The holes for magnets have a little bit of extra room to account for the material expanding while printing. To compensate for the hole being a bit too deep I recommend applying the glue to the sides of the flat cylindrical magnets (the ones in the base) instead of the bottom flat side. It might also be a good idea to insert the flat magnet by attaching it magnetically to the already assembled corresponding modular part (using the modular part as a sort of an applicator).




## How to Operate it
This section will show you how to operate the spooler.

### Loading the Spooler
Loading the spooler with the film is mostly obvious.

1. You have to bring it into a completely dark room or use a changing bag.
2. Pull the film through the narrow light-trap corridor first and then put the spool onto the rod and secure it inside the circle-shaped hole so that it can spin freely.
3. You might want to tighten the film a little bit just so that there's no unnecessary slack.
4. Then you can put the lid onto the body of the spooler and secure it using the screws. You might want to take turns tightening all of them "at the same time" so that there's no unnecessary tension and it all fits together nicely. You want to make sure that the lid is touching the body of the spooler everywhere and there are no gaps. Then you can expose it to the light.


### Using the Spooler
You should have enough space to work within the loading-space of the spooler. The part of the process before you actually start twisting the lever should be straightforward. Then, depending on your preference, you might want to use one of two possible ways to close the door and install the lever into the film canister's core.

5 A. When the canister is in place and the roll of film is connected to it, you need to slide the door in place so that the slots in the turn-key are aligned with the cartridge's core. The door needs to slide all the way down and the bottom of it needs to be aligned with the bottom of the _spooler_. You might need to turn the turn-key gently as you are pressing on it to align it correctly. You should be able to recognise that everything is in place, it all fits together nicely, no slack, no gaps, no misalignment.

5 B. Alternatively, you could first put in place the turn-key without the door. This way you can see that the alignment is right. After the turn-key is in place, you slide the sliding door over it. This requires the turn-key to be in the right position. The key is asymmetrical so pay attention to that.

6. You can start winding the film into the cartridge now. The number of turns is as usual: cca 30 turns for 36 frames but you need to make some slack for the leader and the exposed part of film. When I do cca 32 turns, I get enough film for 37-38 frames when loading the camera outside the dark room. (When loading the film in a dark room, you might get more frames depending on your camera.)

7. When you are done winding, you can position the key so that the door can slide up. You can remove the door, but keep the turn-key in place. _This is a good practice when the fit between the key and the cartridge core is a bit too snug (you'd pull out the cartridge out otherwise and you might not want to do that)._ Then you can carefully disconnect the turn-key and the film cartridge.

8. Finally, you can cut the film and close the loading compartment again. I like to store the turn-key in an inverted position so that it takes less space (you slide the door in first and then you put the turn-key "head-down" into the key-hole).

