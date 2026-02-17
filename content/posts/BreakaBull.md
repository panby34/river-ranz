---
title: "BreakaBull"
subtitle: "The cozy VR game about making tea"
date: 2026-02-16T20:30:00Z
tags: ["VR", "Programming", "Narrative", "AI"]
featured: true
mood: "Focused"
---

Ever heard the phrase "bull in a china shop?" These five words were the inspiration behind *BreakaBull*, a VR game where you play as a bull running a tea shop.

## Why BreakaBull?

*BreakaBull* is a cozy game, but it also has a unique level of difficulty to it. Since you play as a bull, they have to do everything with their hooves. This can range from making tea and serving customers to sweeping and doing soothing chores around the tea shop. The customers are unique, too— they each have their own backstory and will talk to you about their day, their past, their hopes and dreams... every one of them is their own ~~person~~ animal.

## My Contributions

I was onboarded onto the team halfway through development. My main job was to work as the narrative programmer, designing and implementing the systems that brought our characters to life. I mainly focused on new systems for dialogue, friendship, and the social battery mechanic (which limits how many conversations you can have in a day). However, I was also in charge of adding smaller details related to characters, such as order preferences and spawning conditions.

### Order Preferences

```csharp
if (UnityEngine.Random.Range(0, 1) == 0)
    {
        mOrder.type = TeaTypes.BlackTea;
        mOrder.addons.Add(TeaAddons.Milk);
    }
else { mOrder.type = TeaTypes.HibiscusTea; }

mOrder.temp = TeaTemp.Hot;
mOrder.size = TeaSize.Small;
```

{{< coffee-break title="Personality" >}}
The code above was from the initial addition of order preferences to the game. There are only two possible options: black tea with milk or hibiscus tea. Do you know which BreakaBull customer this order belongs to?
{{< /coffee-break >}}

### Narrative

In addition to being our designated narrative programmer, I also contributed to some of *BreakaBull*'s story writing as well! I mainly worked on writing both the Salamander and the Tortoise.

![Concept art of the Salamander](/images/salamander.png) ![Concept art of the Tortoise](/images/tortoise.png)
