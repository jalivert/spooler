# spooler

<img width="400" alt="Screenshot 2025-06-13 at 13 56 24" src="https://github.com/user-attachments/assets/52db9688-6b4d-4a57-bc05-dc3706609a33" />

A film bulk loader for up to 30m of film.

[Here's a link to Fusion 360 project in the cloud.](https://a360.co/4kNz4AA)

> This work is licensed under the **** (TODO: pick one) license. This means that you are free to download and print it for your non-commercial use-cases. Any improvements and modifications have to credit the original work and have to be made available under the same license. This is to ensure that everyone can benefit from other people making the design better in the future. It does not allow commercial use.

------


## Features and Design Decisions
Here are the main design goals and corresponding features of the spooler. The spooler is by no means perfect or absolutely fool-proof or rather—it does not reach the level of polish I imagine from a commercial solution, operating it requires a little bit of dexterity still.
However, I believe it is a step in the right direction and since I am open-sourcing it someone might be able to modify the design and make it even better.
Here are some key features.

### Ease of Use
My goal was to make a bulk film loader that would allow an easy manipulation with the film cartridge. I wanted to have the space where the film canister goes to be as open and accessible as possible. The spooler achieves this by the film canister space being open from the front and top and mostly open from the sides. More details about how to operate the "door-mechanism" in the section on how to operate the spooler.

### Modularity
There are different film producers and they might use differently shaped and sized spools. The film canisters are also little bit different. The canister cores from different manufacturers (the little bit that you twist and roll the film around) have a bit different diameters. This is why the spooler has those two bits interchangeable.

The interchangeable rod that holds the bulk spool has another feature. Because it spins together with the bulk roll of film, the film does not spin on the inside of the spooler and there should be no unnecessary friction. _This is hard to verify as I can not see inside the spooler._

There are files for the spool rod that fits bulk cores from Foma. I don't have access to bulk rolls from Illford or Kodak. Anyone is free and encouraged to either submit the right dimension for other spools or design it and push it into the repository.

### The Lever
The lever used for twisting the film into the cartridge does not need to be held or pushed down for it to stay in place. This way you don't have to worry about accidentally exposing the inside of the loading space in the middle of the process. The key-shaped lever is held in place by friction inside the "door-mechanism". You can learn more about this in the section on operating the spooler.


## How to Print it
I have published print profiles for users of Bambu printers. You can find them here (TODO: add the link).

Users of other printers can download the `step` files and print the parts either using my settings (TODO: add a link to a file with settings and explanations of those) or their own settings should they decide to make adjustments.

> If you need help with printing, you can [open an issue](https://github.com/jalivert/spooler/issues/new/choose) and I will try to help.


## How to Assemble it
One key part of the assembly is gluing enough felt in various places. This section will walk you through it and offer explanation of why the felt is important for both light sealing and correct function. Another key aspect is how the lid is attached to the body of the spooler. To take care of that you will need some extra material and tools.

### What You Need Aside from the 3D Printed Parts
The lid and the body are held together using 7 M3 heat inserts and screws. You will need to buy those.
It seems possible to instead tape the lid and the body together with a black electrical tape. For that, you will need to print the alternative lid with no holes. It should not be necessary, but it's better to be safe than sorry.
If you decide to use the heat inserts, you will need something to heat them with and push them into the body of the spooler.

So here's a list of things you will need:
- [X] 7 M3 heat inserts
- [X] 7 M3x10 screws
- [ ] soldering iron/pen (for heating and inserting)
- [ ] M3 bit


TODO: write


## How to Operate it
This section will show you how to operate the spooler.

### Loading the Spooler
Loading the spooler with the film is mostly obvious.

1. You have to bring it into a completely dark room or use a changing bag.
2. Pull the film through the narrow light-trap corridor first and then put the spool onto the rod and secure it inside the circle-shaped hole so that it can spin freely.
3. You might want to tighten the film a little bit just so that there's no unnecessary slack.
4. Then you can put the lid onto the body of the spooler and secure it using the screws. You might want to take turns tightening all of them "at the same time" so that there's no unnecessary tension and it all fits together nicely. You want to make sure that the lid is touching the body of the spooler everywhere and there are no gaps. Then you can expose it to the light.


### Using the Spooler
You should have enough space to work within the loading-space of the spooler. THe part of the process before you actually start twisting the lever should be straightforward. Then, depending on your preference, you might want to use one of two possible ways to close the door and install the lever into the film canister's core.

5. TODO: write


