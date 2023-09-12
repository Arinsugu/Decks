# GLORY TO THE MANTIS

![alt text](https://images.oracleofthevoid.com/l5r/28/bf/printing_11429_1_details.jpg)

## About the Repo

A collection of Decklists for use with `Sun and Moon` to relive the glory days of L5R CCG, the real card game

## Style Guide

### Deck Names

- `<Legality> <Clan> <Sensei>, <Nickname>` for Post Ivory Legalities
- `<Legality> <Clan> <Stronghold>, <Nickname>` for pre Ivory Legalities
- `<Legality> <Clan> <Sensei/Wind> <Stronghold>, <Nickname>` for legalities with senseis or winds

example: CE MN DGC, Follow Me

### Commit Names and Descriptions

Outside of the initial bulk commit of decks, a commit must only have at most one deck modified per commit.

- Commit Name: `<Deck Name>` as above
- Commit Description: `Details of changes here, what cards were swapped out, etc`

If adding a new deck, then a commit must follow these rules

- Commit Name: `NEW DECK: <Deck Name>` as above
- Commit Description: `Basic Strategy And Ratios`

Should a commit be a non-deck file, then then follow the xkcd rule of commit names and descriptions, which is

![alt-text](https://imgs.xkcd.com/comics/git_commit.png)

### Decklist.txt Format

Legality: `<Legality>`

#### Pre-Deck

`<Stronghold>`

`<Strating Holdings if Any>`
> Applies mainly to Celestial and Emperor legalities

#### Dynasty

`[Personalities]`

> Personalities are separated by their keywords as desired by deck design
They are grouped in order of priority of the following:
>
>1. Keyword Importance in conjunction with fate deck *(e.g. Commanders in the first group of cards if the deck is a **Commander** focused deck)*
>2. **Unique** Keyword
>
example:
in a deck that focuses on commander, the personality list would look like this

```text
Yoritomo Naizen - exp3
Moshi Kalani - exp
3 Yoritomo Zinan
3 Yoritomo Sunagawa
3 Tsuruchi Seisha

Tsuruchi Gidayu - exp
3 Tsuruchi Sanjo
3 Yoritomo Tatsuhiko

Tsuruchi Nobumoto - exp2
Yoritomo Utemaro - exp2
```

`[Holdings]`
> Holdings are grouped by the following priority:
>
>1. **Unique**
>2. Importance in the deck *(if able to change it for tech cards)*
>3. Fortification
>
>>*Fortifications are always at the bottom because I dslike them*

```text
Shrine to Yoritomo
The Imperial Treasury
3 Kobune Port (Celestial)
3 Permanent Encampment
3 Wooden Barricade
3 Newly-Discovered Mine
2 Imperial Artificer
```

`[Celestials, Regions, Events]`
> Non-Holding, Non-Personality Dynasty cards are ordered and grouped by any of the following:
>
>1. Feelings
>
#### Fate Deck

`[Attachments]`

> Attachments are grouped up by the following:
>
> 1. Attachment Type
> 2. Importance in the Deck
> 3. Keywords of importance *(e.g. Weapon)*
> 4. **Unique** Keyword
>

`[Strategies]`

> The only guideline for strategies are to seperately group the staples for the deck and the ones that can be swapped around.
>
> *basically the rule for importance in the deck*
>
> Strategies are suggested to roughly be grouped up by a mix of either preference, usage, and printed abilities

`[Rings]`

> Grouped by real rings, then any fake rings *(e.g. Fudo Rings, Dark Rings)*

#### Notes

Mark the set that the card was released in when it was legal for that arc if it has had any MRPs.
> example: `Creating Order` was given an MRP for Ivory but it was immensely changed, if playing on Celestial or Emperor edition, append (FL) at the end of the card to denote the set for Sun and Moon

As the cards are properly grouped up in an organized manner, it doesnt matter if this style guide is followed strictly. One can have ascending gold cost for non-uniques while at the same time descending gold cost for uniques so long as they group uniques differently from non-uniques.

Or if a decklist has holdings first over personalities, as long as they're grouped together properly and somewhat organized, it is okay, Dynasty first then Fate is important though
then Proxies are always at the bottom.

#### Example Decklist

```text
Legality: Celestial
Dragon's Guard City

Border Keep (Celestial)
Bamboo Harvesters (Celestial)

Yoritomo Naizen - exp3
Moshi Kalani - exp
3 Yoritomo Zinan
3 Yoritomo Sunagawa
3 Tsuruchi Seisha

Tsuruchi Gidayu - exp
3 Tsuruchi Sanjo
3 Yoritomo Tatsuhiko

Tsuruchi Nobumoto - exp2
Yoritomo Utemaro - exp2

Shrine to Yoritomo
The Imperial Treasury
3 Kobune Port (Celestial)
3 Permanent Encampment
3 Wooden Barricade
3 Newly-Discovered Mine
2 Imperial Artificer

I Am Ready
Imperial Census
The New Order (Celestial)

Yoritomo's Guidance

Elite Sentry
The Vengeful
3 Taoist Archer
3 Heavy Elite

3 Ronin Brotherhood
2 Iron Gauntlet Brothers

Creating Order (FL)
Ultimate Sacrifice
3 Know No Fear
3 Muscle and Steel
3 Near Miss
3 A Brave New World
2 Inexorable Defeat
3 Superior Mobility
2 Fearless Defense

3 Retribution
2 Justly Earned Victory

Ring of Water (Celestial)
```
