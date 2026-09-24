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

---

## Results
The build started with a lot of research and planning: figuring out what the cyberdeck should be able to do, finding the smallest and cheapest version of every part, and comparing options before buying. This preparation phase took up a big part of the total project time, especially after the Pi Zero 2 W turned out to be unavailable and the plan had to shift to a Pi 4.

The final hardware setup has a Raspberry Pi 4 fully built into the faux snakeskin clutch. The Waveshare 5 inch touchscreen is connected using flat ribbon cables for both HDMI and USB touch input, which made it possible to fit everything into the small bag. A mini wireless keyboard with a touchpad handles input, and a 3.5mm audio extension gives access to the headphone jack. A second HDMI output is set up so the deck can connect to a beamer.

On the software side, Raspberry Pi OS (64-bit) runs VS Code, GitHub (via SSH), Obsidian, Pure Data, and Chromium. Installing openFrameworks was attempted but did not work in the end, due to compatibility issues between the current Raspberry Pi OS version (Debian Trixie) and the build tools. This remains an open task for later.

The custom mounts were designed in Blender using exact millimeter measurements to fit both the display and the Raspberry Pi and the inside of the clutch. It includes a small extruded name tag on the screen mount, and a repeating "ssss" pattern in a snake-like formation on the Pi mount, referencing the clutch's snakeskin texture. Since the 3D print had not arrived by the submission deadline, an acrylic version was made as a backup: cut and shaped by hand with a saw and a rotary tool with sanding attachments. Once the 3D print arrives, it will be sanded smooth and finished with chrome gel nail polish to match the look of the bag.

--- 

## Bezug zu Cute Studies, Maker Culture, dein Paper
This was my first large solo project involving hardware and physical computing, which made almost every step a genuine challenge. Throughout the process, I regularly watched videos from other creators in the community for guidance, especially from Ube Boobey, whose TikToks often showed alternative ways of solving a problem I was stuck on. For deeper technical questions, particularly around hardware and the Linux command line, which was completely new territory for me, I relied heavily on Claude to explain concepts and debug issues step by step.

The most frustrating part of the process was trying to get openFrameworks running on the Raspberry Pi. After two full days of debugging architecture and build tool incompatibilities, I had to put it on hold for now.

This project sits directly within the context of Cute Studies, maker culture, and the accompanying academic paper on cuteness as a mechanism of access. Beyond the technical build, my goal is to become part of that ongoing discussion: around closed, proprietary hardware, and around the ways that a soft, cute aesthetic can carry an underestimated form of rebellion. I am genuinely looking forward to the conversations this project will spark once I start bringing the clutch to real places, for example running visuals off it at a party.

Future work includes getting openFrameworks running on the Pi, and switching from the Raspberry Pi 4 to a Pi Zero 2 W once it becomes available again. This would finally allow the battery and charging setup to be installed, making the cyberdeck fully wireless and usable without being plugged in.

---

## Lessons Learned
The most important thing I take away from this project is the skill set itself: I now have a real, hands-on understanding of what it takes to build something like this from scratch. Even more important, I lost the fear of touching hardware. I feel comfortable tinkering now, and in a way, I feel like I have genuinely become part of maker culture.

A lot of the technical learning happened through small, specific fixes along the way, from correctly applying scale in Blender to debugging Linux dependency errors. Each of these felt minor in isolation, but together they added up to a much better understanding of how hardware and software actually work together.

Time-wise, I held onto the hope of getting a Pi Zero 2 W for a bit too long, which put some pressure on the final stretch. But I don't think this counts as a lesson about buffer time so much as something that just happened along the way. A cyberdeck is never really finished; there is always something to optimize or customize further. That ongoing, evolving nature is part of what the format is about in the first place.
