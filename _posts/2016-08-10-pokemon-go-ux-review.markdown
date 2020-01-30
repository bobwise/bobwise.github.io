---
layout: post 
title: Pokémon Go
tags: pokemon-go ux
---

![*Pokemon Go*](../../../assets/images/pokemongo/pokemon-go-logo.png)

Once again, the Pokémon franchise has seized the world’s attention and is in the midst of a global resurgence in popularity and profitability.  As of this writing, Niantic’s *Pokemon Go* has been out for about a month.  It has already made more than [$200 million in in-app purchases](https://sensortower.com/blog/pokemon-go-first-month) and has been downloaded more than [100 million times](https://www.engadget.com/2016/08/01/pokemon-go-100-million-downloads/) worldwide.  

*Pokemon Go* has also been victim to some very high-profile technical issues associated with their global launch (is it even possible to be prepared for 100 million users only a month after launch?) and has been criticized for a possessing a sometimes poor user experience.  I’m going to explore some of the UX issues that I personally find frustrating.

# Onboarding #

I want to start by talking about *Pokemon Go*’s poor onboarding experience.  By my count, new account creation involves more than **30** different screens, most of which are a sentence or two of exposition from Professor Willow.  This process guides you through agreeing to the Terms and Conditions, setting up your character name and appearance, catching your first Pokémon, and identifying PokéStops.  This onboarding does NOT explain how to interact with PokéStops, how the Shop works, how gyms work, how to find, catch, or train Pokémon, how to hatch eggs, or how the various items in the game work.

![Professor Willow's Onboarding](../../../assets/images/pokemongo/willow_onboarding.png)

I will say that the onboarding does a good job of describing the AR camera immediately before the first Pokémon battle, and of attempting to convey how to catch Pokémon in the battle minigame.

![Professor Willow's Onboarding](../../../assets/images/pokemongo/camera_and_throw.png)

Once you do get to your first PokéStop, there is nothing on the UI conveying the action the user should take to get their free items.  Similar to the tutorial overlay in the Pokémon battle, this would be a good opportunity to teach the player how to interact with PokéStops.

![Professor Willow's Onboarding](../../../assets/images/pokemongo/pokestop.png)
*What do I do on this screen?*

Also note that once you’ve logged in to a new account, there is no way to skip the tutorial and no way to cancel it.  At one point after the game crashed, I accidentally logged in with the wrong Google account.  The game kicked off the new user workflow, and I couldn’t log out and get back to my main account until I had chosen a unique username for the account I didn’t want, designed my avatar, and chosen my starter Pokémon.

# Terminology and Metaphors #

*Pokemon Go* introduces a lot of new terminology to players for the items in the game.  Populating your fictional world with fictional items is great, but it’s important that players be able to understand what the items are.  A great way to guide players’ understanding is by having fictional items behave similarly to real-world items that players are already familiar with.  However, this can backfire if metaphors are misused.

*Lures*, *Incense*, and *Razz Berries* are all items that do similar things in the game (help you catch Pokémon).

![Lures, Incense, and Razz Berries](../../../assets/images/pokemongo/items.png)

In real life, a lure is an object used to attract animals to you.  In *Pokemon Go*, a *lure* is placed on a PokéStop to increase the likelihood that wild Pokémon will spawn nearby.  This is a good use of the metaphor.  If you know what the word *lure* means, you have a pretty good chance of figuring out what it does in *Pokemon Go*.

Incense is another object that exists in our real world; we burn incense to create an attractive smell.  In *Pokemon Go*, *incense* is used to increase the rate at which wild Pokémon appear nearby.  We don’t use incense to attract real animals, so this metaphor doesn’t quite work.  Knowing what incense is does not help you figure out what *incense* does in *Pokemon Go*.

And then there’s the *Razz Berry*.  Unlike *lures* and *incense*, this item has been given a made up name based on a real word.  But unfortunately, other than the name and appearance, *Razz Berries* and raspberries have nothing in common.  The *Razz Berry* is used to decrease the chance that a wild Pokémon will run away from you.  This metaphor has been misused.  Knowing what a raspberry is does not help you figure out what a *Razz Berry* does.

And what about *Lucky Eggs* and *Pokémon Eggs*?  This is a good example of how an overloaded metaphor can cause confusion.  Only one of these eggs can hatch, and only one of them can go in an *Egg Incubator*.

![Eggs](../../../assets/images/pokemongo/eggs.png)

Metaphors are a great way to give players a head start on figuring out what items do, but those metaphors need to be consistently applied to avoid confusion.

# Good and Bad Tension #

There are two types of tension in a video game.  **Good Tension** is driven by the game mechanics and presents a challenge to the user.  Overcoming this challenge is what makes a game fun.  If a game is not challenging (or too challenging), we won’t derive enjoyment from overcoming it.  Good Tension often has a release that is in the player’s control.

**Bad Tension** can be introduced into a gaming experience when the player finds themselves struggling not against the mechanics of the game, but against the usability of the game itself.  Confusing interfaces, indecipherable error messages, and poor control over the player character all contribute to Bad Tension.  Bad Tension usually cannot be resolved by the player.

When I accidentally logged in with a new email address and found myself trapped in the onboarding flow, that was an example of Bad Tension.  I wasn’t getting enjoyment out of how challenging it was to end the tutorial - I was getting frustrated by my lack of control over the game.  I really needed a way to skip the tutorial or log out without completing it.  Jakob Nielsen calls this type of functionality an [“emergency exit”](https://www.nngroup.com/articles/ten-usability-heuristics/).

Pokémon battles contain another example of Bad Tension.  A colored ring of varying size on top of the Pokémon indicates the likelihood of catching the Pokémon, but there is nothing in the game explaining what the different colors or diameters mean and how they influence the catch potential.

![Throwing a Pokeball](../../../assets/images/pokemongo/throw_ring.png)

# Error Prevention #

Another important aspect of UX Design is error prevention.  The system should either eliminate error-prone situations entirely or present users with a confirmation option before committing to the action in question.

For example, *Pokemon Go* does a good job of preventing accidental Pokémon transfers by confirming with the user before committing to the transfer.  The confirmation message also explains that this action is irreversible.  The only change I would make here is to explain what the transfer will actually accomplish.

![Confirmation before transferring a Pokemon](../../../assets/images/pokemongo/candy_confirm.png)

An example of a situation where *Pokemon Go* does not do a good job of error prevention is with Pokéballs.  The player has a limited number of Pokéball, and can acquire more from PokéStops or from the Shop.  When you are battling a Pokémon and you run out of Pokéballs, there is no way to get more without abandoning the battle and letting the Pokémon escape.  Right now, players need to keep track of how many Pokéballs they have and remember to buy more before going into a battle.  In my opinion, this is an example of Bad Tension.  This is not a meta game where remembering to stock up on Pokéballs is a satisfying challenge.  This is a frustrating experience where I feel like I am being punished for not paying close enough attention.  In fact, Niantic would probably be well served to add the ability to buy more Pokéballs right there during the battle, since that’s when the player is most motivated to spend some money to help them catch that elusive Charizard.

# Unpredictable User Interface #

A very common source of Bad Tension is an unpredictable or unhelpful user interface.  For example, tapping on the map displays a “ripple” indicator, which suggests that this behavior should have some corresponding action in the game.  In other games, we may expect tapping on the map to move our character to that location, or drop a pin, or show us more information about the location.  In *Pokemon Go*, tapping on the map temporarily puts the map into a “swipe to zoom” mode where you can slide your finger around the screen to zoom the camera in or out.  This is not consistent with similar interactions in other games, and there is no feedback in *Pokemon Go* to help us figure out this camera behavior.

The Shop is the area in the game where real-world money can be exchanged for PokéCoins, the digital currency used to purchase in-game items.  The only exception to this is gym rewards.  Gym rewards are given to players for capturing and holding a gym for their team, and the rewards are claimed in the Shop.  Usually you go to the Shop to exchange real money for PokéCoins and items, but in this use case you go to the shop to pick up PokéCoins.

![The Shop](../../../assets/images/pokemongo/shop.png)

A popular theory in the early days following the game’s launch was the idea that tapping on a Pokéball after a failed throw will return that Pokéball to your inventory.  This theory was reinforced by the fact that sometimes Pokéballs disappear with a little popping animation, and sometimes they disappear by just rolling off the screen.  This was further complicated by the fact that the number of Pokéballs you have is constantly appearing and disappearing during Pokémon battles.

![Pokeball Count](../../../assets/images/pokemongo/pokeball_count.png)

# Conclusion #

*Pokemon Go* is a very fun game and ultimately, I don’t expect the UX issues I’ve outlined here to have a big impact on its early success (again, 100 million worldwide users in less than a month).  But once the initial hype has worn off and the game isn’t such a big part of our global culture, poor UX will generate the kind of frustration that drives players away.  For the time being, Niantic’s time is definitely best spent on stability, bug fixes, and rolling out the game to more countries.  But once the launch is complete and the game is stable, quality of life issues will become much more important to players.
