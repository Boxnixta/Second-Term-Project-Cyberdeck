# Second Term Project: Building a cute whimsical Cyberdeck
This project builds a small personal computer into a pink faux snakeskin clutch bag. The idea came from a growing online community of FLINTA, queer creators and allies who started building custom computers into vintage handbags and thrifted cases in early 2026. Where most consumer electronics are sealed, proprietary devices that hide their own inner workings and actively resist repair, these builders reclaim that knowledge by constructing their own machines from scratch. This project is part of that conversation. The computer runs on a Raspberry Pi 4 and includes a 5 inch touchscreen display, a wireless keyboard, and a custom-fabricated screen mount. It is also loosely connected to an academic paper written in the same semester that examines why cuteness works as a way of making tech spaces feel more accessible. The build is presented as a functional prototype and a milestone of an ongoing personal project.

## Concept
The hyperfeminine cyberdeck community felt immediately relevant to me, not just as a research subject but as a space I wanted to actively be part of. Building my own cyberdeck was a way of joining that conversation through making rather than just writing about it. This was also my first physical computing project, which made it both a technical challenge and a personal milestone.

The vision behind this build is practical as much as it is aesthetic. As a DJ who co-organizes parties with my collective, one recurring gap has always been visuals. Good visuals are hard to come by, and bringing your own setup is often complicated. A fully functional computer built into a clutch bag that can connect to a beamer and run audio-reactive visuals on site felt like a solution that is also a statement. A computer in a handbag is, simply put, very badass.

The project sits at the intersection of maker culture, DJ and party culture, and Cute Studies. The clutch is not just an enclosure. It is the concept.

---

## Implementation
The build centers around a Raspberry Pi 4 Model B running Raspberry Pi OS (64-bit), housed inside a Daisy Dixon faux snakeskin clutch bag, sourced secondhand from someone who only wanted the watch it came with.. The display is a Waveshare 5 inch capacitive touchscreen (800x480) connected via a short Micro-HDMI to HDMI ribbon cable, which was a genuine gamechanger for the build: standard cables are too bulky to fit cleanly inside a clutch, and finding flat ribbon cables in the right connector format made the entire assembly significantly more compact and manageable. Touch input is connected via a short USB ribbon cable. Input is handled by a mini wireless keyboard with integrated touchpad via a USB dongle. A custom screen mount fabricated from acrylic holds the display in place inside the clutch, with a 3D-printed version currently in production and awaiting delivery.

The software setup includes VS Code for coding, Obsidian for note-taking, Pure Data for audio work, Git and GitHub for version control, and Chromium as the main browser. SuperTuxKart is also installed, because why not.
Installing Open Frameworks turned out to be a major debugging problem, so I had to put it off until later. 

### Project Reflection (Pi Zero 2 W Teil):

One of the biggest challenges of this project had nothing to do with building: it was finding the right hardware. The original plan was to use a Raspberry Pi Zero 2 W, which would have been significantly smaller and more suitable for the clutch enclosure. However, the Pi Zero 2 W has been out of stock everywhere for months. The few units available on eBay were listed at auction prices of 60 euros and above, compared to a retail price of around 18 euros, which made purchasing one unreasonable. After three months of checking stock trackers and waiting, the decision was made to use a Raspberry Pi 4 as a stand-in. This works well as a development platform and allows the project to be fully functional and documented by the deadline. Switching to the Pi Zero 2 W remains a planned next step once stock normalizes.
