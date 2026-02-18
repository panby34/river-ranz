---
title: "Heart of the Cards"
subtitle: "A dating sim with strategy"
tags: ["Programming", "UI", "Unity", "2D"]
mood: "Energized"
---

*Heart of the Cards* was born from the intersection of dating sims and deckbuilders. For this 3-month project, our team worked to bring the idea to life. Unfortunately, things fell through, and in the end, the project ended up feeling incomplete.

[INSERT KETCHUP RESPONSE]

## Our Intention

We wanted to create something that hadn't been done before. The team was heavy on narrative specialists, and so we absolutely needed to have fun characters and an interesting story. Our game idea was formed fairly quickly, and the team was excited about the prospect of *Heart of the Cards*.

## So... What Happened?

To make a long story short, the design scope was too much. We had only 2 designers on the team, and with all the mechanics and card types available in *Heart of the Cards*, they were stretched too thin. I joined some of the design meetings as a faux designer, but by that point in development, it was already too late. This resulted in a lot of half-baked ideas and unexplained mechanics, which made the game confusing and near impossible to understand. Additionally, because the design scope was so high, progress on programming had to be pushed back, resulting in a very intense programming crunch toward the end of the project. *Heart of the Cards* was eventually cancelled, and the team disbanded.

[INSERT CRINGE]

### What Was Learned?

The main programming challenge in *Heart of the Cards* was data management. Because there are so many ways to categorize cards, we had to be careful with the way we organized them. There were a lot of things that had to be considered during development, and it was easy for wires to get crossed with all the different UI elements we were using. Additionally, because programming process was pushed back, we had to settle for functionality over organization, and as a result, the project scripts ended up messy and confusingly organized.

```csharp
public class Card
{
    public string cardName = "null";
    public string cardDescription = "";
    public Sprite cardSprite = Resources.Load<Sprite>("Sprites/card");
    public int actionValue;
    public GameManager.CardTypes cardType;
    public Sprite cardDesign;

    public int charmValue, cringeValue;
    public ChillMechanic chill;
    public BoostMechanic boost;
    public AddActionsMechanic addActions;
    public DrawCardMechanic drawCards;

    public string questionResponse;
    public string[] cardResponse = new string[] { "", "", "" };

    public bool canBeDiscarded;
}
```

{{< coffee-break title="Class Constructors" >}}
When creating a custom class, you add a constructor. Constructors are an easy way to create a class object. The card class constructor has been omitted from the code snippet above to be succinct, but it was a crucial part of the game's functionality!
{{< /coffee-break >}}

However, I do believe I learned a lot of new skills during my time on the *Heart of the Cards* team. Being part of design meetings allowed me to learn some new game design skills, but also allowed me to work on decision-making and team management. Working with the other programmer on the team gave me the chance to practice my leadership skills, divvying up tasks and checking in periodically during development. I also acted as the sound designer, which was a new discipline for me, but I managed to edit together some free sound assets in a way that fits the game's feel decently well.

### What Would I Do Differently?

If I were to do it all again, I think I would've tried to take on more of a leadership role earlier on in the project. I would've attended more of the early design meetings, gotten those mechanics ironed out, and implemented them. Organization would definitely come more into play— clean, properly named files, and more detailed comments in the code. I also think pushing for the designers to get in-engine would've helped with development, especially once the mechanics were decided on and fleshed out. Adding a real tutorial earlier in development also would've provided a lot in terms of player comprehension, something *Heart of the Cards* was sorely lacking.


While *Heart of the Cards* isn't the most impressive project I've been a part of, I'm still grateful for the experience and all I learned from it. I believe that working on this game taught me a lot and has given me more foresight for scope problems and potential crunch time. I feel more capable in my leadership abilities and teamwork skills as well. I understand how to navigate difficult situations and how to communicate better with teammates about issues that arise during development. Ultimately, *Heart of the Cards* was a helpful learning experience for me, and I'm hopeful that I will be able to use my knowledge to improve any future teams I work with.
