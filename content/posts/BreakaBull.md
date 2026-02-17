---
title: "BreakaBull"
subtitle: "The cozy VR game about making tea"
date: 2026-02-16T20:30:00Z
tags: ["VR", "Programming", "Narrative", "AI", "Unity"]
featured: true
mood: "Cozy"
---

Ever heard the phrase "bull in a china shop?" These five words were the inspiration behind *BreakaBull*, a VR game where you play as a bull running a tea shop.

## Why BreakaBull?

*BreakaBull* is a cozy game, but it also has a unique level of difficulty to it. Since you play as a bull, you have to do everything with your hooves. This can range from making tea and serving customers to sweeping and doing soothing chores around the tea shop. Seems simple enough, right? But the difficulty lies with the hooves— without the luxury of opposable thumbs, every task requires careful consideration and grace. Gameplay is focused on navigating a world that isn't built for you, but without any stressful stakes. Do your best to appease the clientele— or don't. We won't tell.
Every day, customers will come into the tea shop. They're unique, too— each customer has their own backstory and will talk to you about their day, their past, their hopes and dreams... every one of them is their own ~~person~~ animal.

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

![Concept art of the Salamander](/images/breakabull-salamander.png "Salamander concept art") ![Concept art of the Tortoise](/images/breakabull-tortoise.png "Tortoise concept art")

#### The Salamander

When designing the Salamander's backstory, I really wanted to have him seem very carefree and silly. Their tea order is always 100% random, making the Salamander the only customer to not have any specific preference when ordering. This means he can end up with some truly horrific orders, but his laid-back nature allows him to laugh it off and drink it anyway.
Despite the Salamander being a silly, lighthearted character on the outside, they have a lot of feelings. When I started writing his story, I knew I wanted his main arc to focus on themes of community and belonging, and his story pieced itself together from there.

{{< coffee-break title="Names" >}}
Picking names for our characters took some time— [CHOSEN NAME] could've ended up as Sammy, Finn, Monty, or Flavio instead!
{{< /coffee-break >}}

#### The Tortoise

dude i lowkey haven't written her yet. she's an old lady tho
