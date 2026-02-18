---
title: "Nest Quest"
subtitle: "A cute, child-friendly game."
date: 2025-04-19T18:45:00Z
tags: ["Programming", "Narrative", "Unreal Engine", "3D"]
mood: "Hopeful"
---

If there's one thing the *Nest Quest* team loved, it was ducks. We knew from the start that our game needed to involve them in some way, and it didn't take long after that for our concept to come together. We decided to aim for something both children and adults could enjoy, with bright colors, cute sounds, and adorable mechanics. And with that, *Nest Quest* was born.

[INSERT NEST]

## My Role

As one of two programmers for *Nest Quest*, I worked on a number of mechanics for the game. I implemented design ideas, tested them, and fixed bugs as they arose. We only had 3 months to complete this project, and thus it was important to focus on functionality and appearances to give the illusion of what the player expects.

### Creative Solutions

Mid-development, the team decided we wanted to add swimming to the game. However, water physics can get complicated, and with our deadline fast approaching, there was no time to risk on potential bug fixing. Instead, I created an invisible platform under the water's surface and animated it with a slow, wave-like motion. When the player gets in the water, it simulates the slow bobbing motion you would expect from swimming, but without any extra physics or mechanics involved.

[INSERT DUCK IN WATER]

### Duckling AI

One of the things we knew we wanted was a gaggle of little ducklings to follow the player around. After collecting a duckling, it would start to follow the player, just like in real life! Designing the pathfinding and navigation AI for the duckling was my task, and it proved to be more difficult than expected. I was new to Unreal Engine and 3D game development, but with a ton of research and more trial-and-error than I'd like to admit, the current duckling AI was born. It has some flaws, but I implemented several features to help mitigate that.

- **Teleportation**. The player, as an adult duck, can move faster than the ducklings. Usually, this isn't much of an issue, but if the player chooses to sprint constantly, ducklings are likely to get left behind. Not only that, but being so small, they easily get caught on obstacles and and unable to free themselves. This issue proved difficult, so I added in that ducklings could teleport to the player if they got too far away. This way, there's no more lost ducklings!

[INSERT TELEPORT DUCKLING GIF]

- **Gravity**. The player can glide in the air using their wings. The ducklings don't have that same ability, but we don't want to leave them behind! I ended up turning off the gravity on ducklings, which allows them to follow smoothly behind the player, no matter how high up they may be. This also causes the issue of ducklings floating slightly above the ground, which unfortunately was unable to be patched out before the deadline.

[INSERT DUCKLING GLIDE GIF]
