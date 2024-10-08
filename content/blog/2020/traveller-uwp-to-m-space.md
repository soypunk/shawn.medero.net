---
title: Traveller Universal World Profiles to M-Space Planets 
date: 2020-01-20T11:00:00-07:00
summary: A step-by-step guide to converting a Traveller Universal World Profile (UWP) to material that can be used with M-Space
tags:
- M-Space
- rpg
- Traveller
aliases:
- /2020/1/traveller-universal-world-profiles-to-m-space-planets
---

Traveller is well known for it is various "universal codes." The Universal Character Profile/Universal Personality Profile was a shorthand method to quickly describe a character's characteristics. The Universal Planetary Profile/Universal World Profile (UWP) describes the qualities of a world. In this article I want to take at look at how you can map a UWP to an M-Space Planet so that you can reuse Traveller-specific mapping tools with M-Space. It will not be always be a one-to-one mapping and there will be some judgements you'll have to make for your game.

## UWP code in a nutshell

A UWP code looks like this: `C77A9A9-6`

1. Starport: C
2. Size: 7
3. Atmosphere: 7
4. Hydrographics: A
5. Population: 9
6. Government: A
7. Law level: 9
8. Tech level: 6

There are some other details sometime included separately from this main code sequence but these are the primary attributes we will be considering.

## Starports

Starports map over fairly cleanly. Traveller has some specific ideas about "annual maintenance" that may or may not fit into your own M-Space game depending how closely you are tracking such details.

| UWP Starport Code | UWP Descriptor | M-Space   | Shipyard Capacity  | Maintenance |
| :---------------: | :------------- | :-------- | :----------------- | :---------- |
|         A         | Excellent      | Full      | Build & Repair     | Yes         |
|         B         | Good           | Standard  | Repairs & Upgrades | Yes         |
|         C         | Routine        | Local     | Simple repairs     | Yes*        |
|         D         | Poor           | Emergency | None               | No          |
|         E         | Frontier       | Emergency | None               | No          |
|         X         | None           | None      | None               | No          |

* Typically Routine/Class C Starports were not capable of performing "annual maintenance" but could do simple maintenance.

## Size

Traveller world sizes starting at size 6 map over cleanly to M-Space, but sizes 0-5 are not covered. To help explain the lack of designations at the lower sizes, it is important to note that world sizes 1-4 would have such low gravities that walking in a straight line would be problematic.

| UWP Size Code | Traveller World Size           | Traveller Gravity | M-Space     |
| :-----------: | :----------------------------- | :---------------- | :---------- |
|       0       | 800 km (typically an asteroid) | Negligible        | -           |
|       1       | 1,600 km                       | 0.05              | -           |
|       3       | 3,200 km                       | 0.15              | -           |
|       5       | 4,800 km                       | 0.25              | -           |
|       7       | 6,400 km                       | 0.35              | -           |
|       9       | 8,000 km                       | 0.45              | -           |
|       2       | 9,600 km                       | 0.7               | Extra Small |
|       4       | 11,200 km                      | 0.9               | Small       |
|       6       | 12,800 km                      | 1.0               | Medium      |
|       8       | 14,400 km                      | 1.25              | Large       |
|    10 (A)     | 16,000 km                      | 1.4               | Extra Large |

## Atmosphere

M-Space includes some tables for Atmospheric Pressure and Breathability which we will use to translate back to a UWP code.

| UWP Atmosphere Code | Descriptor         | M-Space Pressure | M-Space Breathability |
| :-----------------: | :----------------- | :--------------- | :-------------------- |
|          0          | None               | None             | None                  |
|          1          | Trace              | None             | None                  |
|          2          | Very Thin, Tainted | Too thin         | Vacuum Suit           |
|          3          | Very Thin          | Too thin         | Vacuum Suit           |
|          4          | Thin, Tainted      | Thin             | Breathing mask        |
|          5          | Thin               | Thin             | Breathing mask        |
|          6          | Standard           | Earth like       | Earth like            |
|          7          | Standard, Tainted  | Earth like       | Breathing mask        |
|          8          | Dense              | Dense            |                       |
|          9          | Dense, Tainted     | Dense            | Breathing mask        |
|       10 (A)        | Exotic             | Varies           | Vacuum Suit           |
|       11 (B)        | Corrosive          | Varies           | Vacuum Suit           |
|       12 (C)        | Insidious          | Varies           | Vacuum Suit           |
|       13 (D)        | Dense, High        | Dense            |                       |
|       14 (E)        | Thin, Low          | Thin             | None                  |
|       15 (F)        | Unusual            | Varies           | Varies                |

It is important to note that while Dense worlds may not require a particular Breathing mechanism they would be rather hot and have violent electrical storms, continent-sized hurricanes, or massive hailstones.

## Hydrographics

Traveller does a whole thing with Hydrographics and has a system for generating a climate profile given a few inputs. For example, a Size code of 6-8, an Atmosphere 5, 6 or 8 and Hydrographics 5-7 might give you a "Garden World." 

There is no easy conversion here other than to provide some guidance on the codes and allow you to think about how close the planet might be to the habitable zone and what effect that would have on the climate.

| UWP Hydrographic Code | Descriptor                                 |
| :-------------------: | :----------------------------------------- |
|           0           | Desert world                               |
|           1           | Dry world                                  |
|           2           | A few small seas.                          |
|           3           | Small seas and oceans.                     |
|           4           | Wet world                                  |
|           5           | Large oceans                               |
|           6           |                                            |
|           7           | Earth-like world                           |
|           8           | Water world                                |
|           9           | Only a few small islands and archipelagos. |
|          10           | Almost entirely water.                     |

Here's some general guidance as to how you can fit all of the codes together:

| World Class | Size             | Atmosphere             | Hydrographics | Temperature       |
| :------------ | :--------------- | :--------------------- | :---------- | :---------------- |
| Rock        | 0                | 0, 1, 2, 3             | 0           | -                 |
| Harsh       | 1, A+            | 4, 7, 9, A, B, C, D, F | 1, 2, 9, A  | Freezing, Boiling |
| Marginal    | 2, 9             | 5, 8                   | 3, 4, 8     | Hot, Cold         |
| Garden      | 3, 4, 5, 6, 7, 8 | 6, E                   | 5, 6, 7     | Temperate         |

* Table courtesy of [Daniel Stevens](https://www.freelancetraveller.com/features/preproom/loprep.html)

## Population

At this point we need to jump out of M-Space's World Building chapter and head to the previous chapter on Alien Creation. Mapping Traveller's population code to M-Space's population descriptors requires a bit of judgement as to what "medium" means in your universe. Here's an idea as to how one might do that:

| UWP Population Code | Descriptor            | M-Space Descriptor |
| :-----------------: | :-------------------- | :----------------- |
|          0          | None                  | None               |
|          1          | Few                   | Very Low           |
|          2          | Hundreds              | Very Low           |
|          3          | Thousands             | Low                |
|          4          | Tens of thousands     | Low                |
|          5          | Hundreds of thousands | Medium             |
|          6          | Millions              | High               |
|          7          | Tens of millions      | High               |
|          8          | Hundreds of millions  | Very High          |
|          9          | Billions              | Very High          |
|       10 (A)        | Tens of billions      | Super-dense        |

## Government

Governments in Traveller are rather specific compared to the broader terms used in M-Space. Additionally M-Space's Circle mechanic provides a richer way to represent these planetary governments within your game world and how their actions can influence or impact your players. There's no reason why you could not use Traveller's label in your M-Space game. Some GM fiat is necessary to determine what these labels mean in your game, but here's a sample mapping if you wish to preserve M-Space's labels.

| UWP Government Code | Descriptor                  | M-Space Ruler                 |
| :-----------------: | :-------------------------- | ----------------------------- |
|          0          | None                        | None, Anarchy                 |
|          1          | Company/Corporation         | Dictatorship, Semi-Democratic |
|          2          | Participating Democracy     | Democracy                     |
|          3          | Self-Perpetuating Oligarchy | Dictatorship                  |
|          4          | Representative Democracy    | Semi-Democratic               |
|          5          | Feudal Technocracy          | Council                       |
|          6          | Captive Government          | Council, Dictatorship         |
|          7          | Balkanization               | Many                          |
|          8          | Civil Service Bureaucracy   | Council                       |
|          9          | Impersonal Bureaucracy      | Council                       |
|       10 (A)        | Charismatic Dictator        | Dictatorship                  |
|       11 (B)        | Non-Charismatic Leader      | Dictatorship                  |
|       12 (C)        | Charismatic Oligarchy       | Dictatorship                  |
|       13 (D)        | Religious Dictatorship      | Dictatorship                  |
|       14 (E)        | Religious Autocracy         | Dictatorship                  |
|       15 (F)        | Totalitarian Oligarchy      | Dictatorship                  |

M-Space provides two additional layers of descriptors called Foreign Policy and Conflict Intensity that would require you to know a bit more about your world's backstory in order to determine how your planetary governments are functioning with their neighbors.

## Law level, 

M-Space has a 1:1 mapping for Traveller's Law Levels 0-9. These can be found in M-Space on page 134 in the Alien Creation chapter.. The table presented here could be slightly cleared that the Weapons column is saying what is "restricted." So, Level 9 does not mean "Any Weapons" are allowed but that all weapons are restricted by the government.


## Tech level

M-Space has a 1:1 mapping for Traveller's Tech Levels 0-15, and you can read a bit about this on page 135, of M-Space's Alien Creation chapter.

So there you go, M-Space is not shy about pointing out its roots from Traveller. In many cases mapping the terminology is not strictly necessary but it can be helpful to your players if they are not familiar with Traveller but own their own copies of M-Space.