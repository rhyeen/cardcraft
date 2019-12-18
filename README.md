# Sharded Cards

## What is Sharded Cards?

### Game Mechanics

Sharded Cards is an online deck building, card building, trading card game.  In the game, you can either face off against the Dungeon: a series of opposing cards that increase in difficulty (much like [Slay the Spire](https://store.steampowered.com/app/646570/Slay_the_Spire)), or you can climb the ranks by facing another player in one of several competitive modes.

The core concepts behind Sharded Cards "deck building" and "trading card" mechanics are well known, but Sharded Cards elevates the play experience by also inviting the player to build their own cards.  Let's take a typical Dungeon Delve as an example:

> You begin the game with a deck of core cards, which are cheap predefined cards that help you survive the first few rounds against the Dungeon's monsters.
> At the end of each turn, you will be able to start building new cards to add to your deck. Cards can be minions that you can place on the playing field to fight against the opposing Dungeon monsters, or spells that can be cast from your hand.
> Cards can also be modified by increasing their basic stats: health, attack, etc, or by giving cards special abilities, such as "Stun", which can prevent a Dungeon monster from attacking. Be frugile though, every modification to the card increases its cost to play.
> Once the modifications are complete, you can add the card to your deck and use it to conquer the Dungeon!

### Technical Details

Sharded Cards has other interesting concepts not seen in typical online card games. 

Foremost, Sharded Cards is playable directly within the browser and can be played on any device that has access to the internet.  This is because the game is actually a web app built following the [Open WC Standards](https://open-wc.org/) and backed by [Google's Firebase](https://firebase.google.com/).

In the spirit of transparency, the code for the game is entirely *viewable* (**not** *[copyable](https://choosealicense.com/no-permission/)*) on Github.  This is partially because we encourage players with a developer background to [contribute](https://github.com/rhyeen/shardedcards/issues/2) if they are interested, and partially because we want to ensure players that different "random" aspects of the game (e.i. drawing cards, obtaining rare items, Dungeon difficulty, matchmaking) are fair and do not exploit addictive tendencies (such as spontaneous in-app purchases to gain a competitive edge).

## Contributing

If you're interested in contributing, please post your interest on [this issue](https://github.com/rhyeen/shardedcards/issues/2) or Slack @rhyeen direclty on the [Shardrealms Slack Workplace](https://join.slack.com/t/shardrealms/shared_invite/enQtMTg5OTg2NjE3MTkwLWM0YTRhYTdhZDA1NDJhNjczZjYwNTQ4MzAzYWIwN2EwZjg3ZWM0NDU1M2E1NTMwZTEwNjE1MDIwMmI5ZWM4N2U).

You can also see a rough roadmap and scratchboard of ideas in the [Projects](https://github.com/rhyeen/shardedcards/projects) section.

Here are a list of all the active repos for this project:
* [Frontend app](https://github.com/rhyeen/sc-app): Written in VanillaJS, [lit-html](https://lit-html.polymer-project.org/), and [lit-element](https://lit-element.polymer-project.org/)
* [Backend serverless functions](https://github.com/rhyeen/sc-functions): Written in VanillaJS and [Firebase](https://firebase.google.com/)
* [Shared types and business logic](https://github.com/rhyeen/sc-types): Written in Typescript. This is used to share functionality between the frontend and backend.
* [Admin app](https://github.com/rhyeen/sc-admin): Used to perform admin-level functions, such as modifying monster cards in a Dungeon.
