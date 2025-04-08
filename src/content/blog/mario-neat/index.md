---
title: "Building a Genetic Algorithm from Nothing to play Super Mario Bros"
description: "This took 7 months during COVID-19."
date: "Feb 12 2022"
---

![Mario-NEAT Demo](/mario-neat.gif)

In February 2022, I made a machine-learning genetic algorithm built from the ground up using research from the University of Texas-Austin "Neural Evolution of Augmenting Topologies" capable of playing and completing a real Super Mario Bros 1-1 ROM utilizing a Nintendo Entertainment System emulator. This project has been awarded "Best Technical Skills" from the <a target="_blank" aria-label="Rutgers University Computer Science Department" href="https://www.cs.rutgers.edu/">Department of Computer Science at Rutgers University</a> on April 17, 2023.

## How did I do it?

With determination and passion, I've always been interested in programming and saw one of my friends, Ryan Park, who was very interested in facial recognition using AI.
Admittedly this is not an original idea of mine, as a YouTuber named SethBling made this very project himself called <a target="_blank" aria-label="MarI/O" href="https://www.youtube.com/watch?v=qv6UVOQ0F44">MarI/O</a> and I remember he published a video like this a long time ago at the time and was wondering if I could achieve this very thing he made using tutorials on YouTube, the scholar article he used, and a different emulator (so that I wasn't directly copying him). I managed to complete the project in a few months.

## Known Bugs

After I finished the project, I wanted to show it off to some of my teachers at my high school and some were very impressed. There was a slight problem though: when replaying a successful genome, it seemed as if when the emulator lags a couple of frames and my script doesn't send its controller inputs and goes out of sync, which makes it unable to complete the replay. This mostly depended on if I used my home server vs my laptop at the time to train my network of genomes.

