# Twine prototype

- ~~Write skeleton scenes about three spaces deep in either direction from CT spawn~~
- ~~Write skeleton CT bodies into deepest space (maybe Bombsite B? We'll see.) (Consider making this dynamic in future iteration.)~~
- ~~Hard-code skeleton terrorist encounter into a space, maybe complete with random numbers for missing and dying, hitting and winning~~ (Currently just with a deterministic kill of the terrorist.)
- ~~Add descriptive expansions to two corpses (T and CT)~~ (Currently just the terrorist corpse)
- ~~Language pass to figure out agency and "I statements" etc.~~ (Think this is mostly in place, writing the thing helped a lot here.)
- ~~Language pass to get some feeling into it?~~ (Not sure this is wise?)
- ~~Another writing pass based on current understanding of the game~~
- ~~Do a performance to get a sense of what the feeling of play might actually be~~
- ~~Rewrite scenes based on minimising text, minimising link length (in conversation with testbed work below in terms of the link texts).~~ (Didn't do this - honestly I think I miiiight be done with the Twine prototyping now? Need to start working out my own UI.)

# annyang prototype

- ~~Build a basic project structure with annyang included (and working)~~
- ~~Simulate a sequence of voice commands with text responses on screen (in an array or whatever)~~
- ~~Test it out and write about it~~
- ~~Polish the prototype with some nicer looking typography~~
- ~~Try adding some "what I heard" feedback (at least when it's wrong)~~ (This is going to be really hard since the annyang wildcarding thing seems to override more specific commands.)
- ~~Complete the scene properly with the dead terrorist in the final scene (just fake it)~~

# annyang command testbed

- ~~Build a simple prototype that lets me (and others) try out a whole bunch of relevant commands~~
- ~~Try it out~~
- ~~Reflect on it~~
- ~~Send it to J+M and Rilla~~
- ~~Reflect on tester feedback~~
- ~~Build ability to trace out failed attempts~~

- ~~Turn it into a more thorough testbed where it progressively asks you to try a command three times then turns it into a link after the third fail (stores the interpreted phrases), gives visual feedback when it hears you say something that doesn't work~~
- ~~Get it to print out a diagnostic page at the end with stats, failed phrases, etc.~~
- ~~Rewrite a series of relevant phrases (related to the world and game) that avoids suspected problem phonemes and words~~ (I did do that.)
- ~~Send it to J+M again~~

# Full Twine prototype

- ~~Establish distinct spaces~~
- ~~Put together a Twine with a passage for every distinct space in the game~~
- ~~Take reference images of every location and terrorists (dead and alive) and CTs~~
- ~~Write basic text and linking for every space~~
- ~~Write sample terrorist encounter with kill sequences that allow testing multiple encounters~~
- ~~Implement persistent corpses~~
- ~~Implement characteristic walls/shapes for terrorist encounters~~
- ~~Use a single variable to track terrorists killed and use that to denote game over~~
- __DOESN'T SEEM TO BE A THING?__ ~~Find a one-page Twine theme?~~
- __COLOURS AND FONT__ ~~Implement some basic CSS/visual styling for presentation of the prototype~~
- __ITALICS WHEN YOU SEE THEM__ ~~Different typography for terrorist texts?~~
- ~~Do final testing of the robustness of this thing~~
- __DID THIS ON FRIDAY 16th__ ~~Send to testers~~

# Failure UI

- __SEEMS KIND OF ROBUST?__ ~~Consider pausing/starting annyang between passages as a way to conceivably avoid the shutdowns it does sometimes when it gets confuse? (Can you unconfuse it?)~~
- ~~Improve the transition on a successful phrase~~
- Improve the overall typography, margins, colours (dim prior texts and highlight current?)
- __THIS SEEMS GIMMICKY?__ ~~Recording the voice input and allowing them to download it? (Would be an amazing sound file... don't know about the storage issues.)~~
- ~~Start with annyang prototype and start figuring out nicer UI stuff~~

# Game design

- __NO LONGER SEEMS NEEDED__ ~~Attempt a more formal writing of the system's dynamics (e.g. terrorist spawning, movement, stealth, cover, etc.)~~

# Implementation

- ~~Create every area and allow transitions between them (no descriptions for now)~~
- ~~Translate Twine areas and commands into JSON for my version~~
- ~~Implement short descriptions (e.g. every area has a short description + a visited tag + an "I look around" command if visited that shows the full description)~~
- ~~Remember the idea of locations with tagging for no encounters~~
- ~~Create a version that has separate pages with fades (or something) between them, but tracks the full story as well~~
- ~~Add ability to display shootings either in-line, all on a new page, or each on a new page~~
- ~~Implement encounters (separate JSON, add text to location at the end)~~
- Encounters
  - ~~Make all three possible~~
  - ~~Add idea of physical object templated in (just make a custom one of my own? [[object]]?)~~
  - ~~Add corpse description to the location and add no_encounters property to it too~~
  - ~~Need to maintain current encounter if it happened and then they "look"!~~
  - ~~Change from "a" to "the" after first viewing of a terrorist?~~
  - ~~Figure out probabilities (including spatial awareness if needed)~~
  - ~~Implement basic probability stuff for terrorists~~
  - __WHY BOTHER?__ ~~Make dynamic gun description stuff (e.g. pistol pointed at you or not, saw you or not, etc.)~~
- ~~Implement mishearing shake~~
- ~~Implement clickable after three attempts (then remove it after the click)~~
- __NO, THEY CAN GIVE UP IF THEY WANT TO GIVE UP__ ~~Implement some kind of "let's give up?" after three clickables?~~
- ~~Add a start passage which is an explanation of the game, with a single command that takes you to the opening scene. (It would be nice to make this a special case that fades out and then into the game so it's not visible at the top of the screen)~~
- ~~Add basic error handling for permission denied, browser denied, no speech available...~~

# Bugs

- __IT WAS TO DO WITH SCROLLING__ ~~Weird delay seems to start appearing the deeper you go especially in kill sequences?~~
