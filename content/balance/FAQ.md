---
date: '2022-02-07'
authors: ["Chicken, Jundarer"]
published: true
patch: "9.2"
title: Patch 9.2 FAQ
sidebarTitle: "Quicklinks"
sidebarContents:  |
  [1. News](#news)
  
  [2. Rotation](#rotation)
  <br>[Openers](#openers)
  <br>[What is my AoE priority?](#aoe)
  <br>[What is my Single Target rotation?](#st)
  <br>[What is my filler priority inside CA?](#filler)
  <br>[How do I use instant Starfire procs from Owlkin Frenzy?](#owlkin-frenzy)
  <br>[Do our dots snapshot?](#snapshot)
  
  [3. Flexible Setups](#setup)
  <br>[What is Balance Druids stat priority?](#stats)
  <br>[What Trinkets should I use?](#trinkets)
  <br>[What Talents should I run?](#talents)
  <br>[T50 row choices and playstyle (9.1)](#t50)
  <br>[What Conduits should I pick?](#conduits)
  <br>[What Soulbinds should I pick?](#soulbinds)
  <br>[What potions should I use?](#potions)
  
  
  [4.Meaningful Choices](#meaningfulchoice)
  <br>[What Legendaries should I craft?](#legendaries)
  <br>[What slot do I craft legendaries in?](#legendaries-slot)
  <br>[What Covenant should I pick?](#covenant)
  <br>[What Domination Sockets should I use?](#domination-sockets)
  
  [5. Covenant specific tips](#covenants)
  <br>[Night Fae](#nightfae)
  <br>[Venthyr](#venthyr)
  <br>[Kyrian](#kyrian)
  
  [6. Miscellaneous](#Miscellaneous)
  <br>[Useful CA + Convoke + Trinket macro](#swifty-macro)
  <br>[How does IQD work?](#iqd)
  <br>[What is Astral damage?](#astral-damage)
  
  [7. Mythic+](#M+)
  <br>[Why am I doing low damage?](#low-dmg)
  <br>[M+ Talents](#M+Talents)
  <br>[M+ Soulbinds](#M+Soulbinds)
  <br>[M+ Domination Sockets](#M+Sockets)
  <br>[M+ Anima Powers](#M+Anima)
  <br>[How to Improve in M+](#M+Improve)
  
   [8. Utility](#Utility)
---

<details>
<summary>Changelog</summary>

 + 2022-02-07:
<br>Updated: Conduits, Talents, Covenants
  
 + 2022-02-05:
<br>Removed: M+ Pre Key ramp
  
+ 2022-02-03:
<br>Added: Utility
<br>Updated: PTR Changes with KA nerf
  
+ 2022-01-12:
<br>Added: Deep Allegiance
<br>Updated: Stellar Inspiration, Precise Alignment, Umbral Inspiration
  
+ 2022-1-11:
<br>Added: Changelog
<br>Updated: Kyrian cleanup
  
+ 2021-12-28:
<br>Added: Tier set opener, Kyrian KA build, KA spreadsheet
<br>Updated: Coundit section (SI,PA), Legendary stats+slots, hyperlinks for legendaries
  
</details>
   
<div id="news">

# [1. News:](#news)

</div>



## 9.2 PTR Changes

9.2 PTR is here and brings some additions to every spec. Everyone is getting their covenant legendary equipable for free, which means all covenant abilities are enhanced baseline. It is to note that this does not mean more choices since you can still only choose one legendary freely.\
On top of this the first iteration of every set bonus has been revealed, ours being the following:

**2-Set -  {{< spell 364423 "Celestial Pillar" >}}:**\
Entering Lunar Eclipse creates a {{< spell 211545 "Fury of Elune" >}} at 25% effectiveness that follows your current target for 8 sec.\
*Notes:* This gives 40 AP. If multiple Celestial Pillars proc at the same time (lunar>inc>pulsar), then the duration of the first pillar will be extended (24sec). The self casted FoE is a different entity and does not affect this.

**4-Set -  {{< spell 363497 "Umbral Infusion" >}}:**\
While inside any Eclipse, the cost of {{< spell 78674 "Starsurge" >}} and {{< spell 191034 "Starfall" >}} is reduced by 20%.\
*Notes:* This stacks multiplicatively with {{< spell 339949 "Timeworn Dreambinder" >}} and does not reduce progress per Astral Power spend for
{{< spell 338668 "Primordial Arcanic Pulsar" >}} (still gives 30ap and 50ap respectively towards Pulsar).


We have also received class changes:

**{{< item 355315 "Sinful Hysteria" >}} :** Now extends Ravenous Frenzy by 0.1s per cast down from 0.2s and lingers 3s down from 5s.
*Notes:* This is roughly a 10% total dps nerf to Venthyr in most situations.

**{{< item 364815 "Kindred Affinity" >}} :**  Now 6%/12% self (from 8%/16% self) and 3%/6% partner (from 8%/16% partner) for NF, NL and VE bonds. Kyrian bond is now 210/420 self (from 150/300 self) and 105/210 partner (from 150/300 partner).
*Notes:* Kyrian got nerfed and it is on par with venthyr in RAID dps in an optimal scenario. In a progress scenario you will most likely not touch it because of how much it loses in an actual encounter. Venthyr and Night Fae will most likely be swapped around depending on encounter (more informations below).

### Analysis:

With how the sets currently work, they will heavily favour one legendary,
{{< spell 338668 "Primordial Arcanic Pulsar" >}}, since both set bonuses heavily synergize with it.\
The 2-Set Celestial Pillar procs its Fury of Elune every time Pulsar is procced which in turn resets your Eclipse and allows for even more Lunar Eclipses.\
The 4-Set Umbral Infusion may reduce the Astral Power you have to spend on Starsurge and Starfall but Pulsar still gets the original cost. A 24 cost Starsurge for example would still progress your Pulsar buff by 30.

Looking at covenants, assuming 2 Legendaries and 4 Tier Piece, Venthyr, Night Fae and Kyrian are all very close to eachother. Since Venthyr and Night Fae both have superior signature abilties (Door of Shadows and Soulshape) and generally better soulbinds you will be switching between them depending on the encounter. Kyrian can still be played without losing much damage but is not recommended. Some preliminary information about what covenant to pick for specific bosses are in the raid guide. 

Simulationcraft has been updated for PTR changes and the APL has also received updates meaning you can sim the legendary changes and set bonuses using Raidbots. Additionally, our sim site will be kept updated whenever more changes come and can as always be found here: https://balance-simc.github.io/Balance-SimC/. You can run the sims yourself by double-clicking on any combination on that site and pasting the result into an Advanced sim on Raidbots. The most recent version of the PTR APL can be found here: https://github.com/balance-simc/Balance-SimC/blob/master/balance_ptr.txt. Feel free to look at the sims and sample sequences and in case anything looks out of line or wrong don't hesitate to tell us.

For the sake of PTR testing and due to the fact that the baseline legendary won't be available for very early progress this is how the covenants match up: https://www.raidbots.com/simbot/report/fBk7jyHc9qsYV8gn5Q8Dyc All Covenants will use Pulsar once you get 2 set and before that Venthyr uses Sinful Hysteria instead.

### Known bugs:

These bugs are known and will be fixed in a later ptr cycle.

- Lunar Eclipse -> Pulsar procs FoE instead of a Celestial Pillar causing you to lose the AsP gain from a manually cast FoE since they do not stack.
  
<div id="rotation">

# [2. Rotation:](#rotation)

</div>

<div id="openers">

## [Openers](#openers)

</div>

Venthyr - with {{< spell 202430 "Nature's Balance(NB)" >}}:<br/> {{< spell 190984 "Wrath" >}}, Wrath, {{< spell 194153 "Starfire" >}}(combat starts half-way through the cast), dots, with NO Bloodlust: Starfire until 90+ AsP, {{< spell 102560 "Incarnation" >}}, {{< spell 323546 "Ravenous Frenzy" >}}, Wrath until max AsP if not there already, {{< spell 78674 "Starsurge" >}} 1x


Night Fae - with {{< spell 202430 "Nature's Balance(NB)" >}}:<br/> {{< spell 190984 "Wrath" >}}, Wrath, {{< spell 194153 "Starfire" >}}, dots, {{< spell 194223 "CA" >}}, {{< spell 78674 "Starsurge" >}} 2x, {{< spell 323764 "Convoke" >}}, Starsurge until you have no more AsP, New Moon, Half Moon, Starsurge, Full Moon
 

Kyrian - with {{< spell 202430 "Nature's Balance(NB)" >}}:<br/> {{< spell 190984 "Wrath" >}}, Wrath, {{< spell 194153 "Starfire" >}}, dots, {{< spell 194223 "CA" >}}, Empower Bond, {{< spell 78674 "Starsurge" >}} 2x, New Moon, Half Moon, Starsurge, Full Moon
  
 
In raid with 2-Set -  {{< spell 364423 "Celestial Pillar" >}} and {{< spell 202430 "Nature's Balance" >}}:<br/> {{< spell 190984 "Wrath" >}}, Wrath, dots, Wrath, {{< spell 194223 "CA" >}}, continue with the openers above.
  
 
Notes:

In raid with {{< spell 202430 "Nature's Balance" >}} first 12 Astral Power gets reset to 50.

Start casting from max range at ~3.5-4 sec without {{< spell 364423 "Celestial Pillar" >}}.
Start casting from max range at ~2 sec with {{< spell 364423 "Celestial Pillar" >}}.


<div id="aoe">
 
## [What is my AoE priority?](#aoe)

</div>

**Venthyr specific notes will be marked with (V) at the start of a point and Night Fae specific ones will be marked with (NF)**

**AoE starting at 2 targets:**

**Any situation:**

- Keep up {{< spell 93402 "Sunfire" >}} as long as your targets will live for another ~10 seconds (the amount of time is reduced per target hit).

- Keep up {{< spell 191034 "Starfall" >}} at all times or use on cooldown with{{< spell 202354 "Stellar Drift" >}} .

**Outside any Eclipse:**

- Refresh {{< spell 8921 "Moonfire" >}} outside of Eclipse if and only if ALL of the following are true:
    - The next eclipse you will enter is Lunar Eclipse
    - All targets can be hit by {{< spell 194153 "Starfire" >}}
    - There are 5 or less targets (10 or less with {{< spell 281847 "Twin Moons" >}}).
    - All targets will live through the entire Lunar Eclipse
    - You will not lose {{< spell 191034 "Starfall" >}} uptime.

- Enter the next Eclipse if in no Eclipse, preferring Lunar Eclipse.

**Lunar Eclipse and both Eclipses (CA/Inc):**

- Use {{< spell 78674 "Starsurge" >}} to stop yourself from overcapping AsP until 6 targets at which point you should overcap.

- Refresh {{< spell 8921 "Moonfire" >}} if you are at 4 (8 with {{< spell 281847 "Twin Moons" >}}) targets or below if the targets will live through the next Eclipse.

- Cast {{< spell 194153 "Starfire" >}}.

**Solar Eclipse:**

- Use Starsurge to stop yourself from overcapping AsP.

- Keep up {{< spell 8921 "Moonfire" >}} on up to 10 targets (20 with {{< spell 281847 "Twin Moons" >}}) if they will live through the next Eclipse and you won't lose {{< spell 191034 "Starfall" >}} uptime.

- Starfire when 5 targets can be hit by it, increased by 1 target for every 20% mastery you have.

- Cast {{< spell 190984 "Wrath" >}}.

**BEFORE cooldowns:**

- If the pack will last more than 35s put {{< spell 8921 "Moonfire" >}} on up to 8 targets (16 with {{< spell 281847 "Twin Moons" >}}). This happens very rarely but is a gain in case it happens.
- (V) Refresh {{< spell 93402 "Sunfire" >}} so you only have to refresh it once during Cooldowns.

**(V) DURING {{< spell 323546 "Ravenous Frenzy" >}}:**
- Refresh {{< spell 93402 "Sunfire" >}} during pandemic(30% of base duration).
- Keep {{< spell 191034 "Starfall" >}} up at all times or on cooldown with {{< spell 202354 "Stellar Drift" >}}. Try to time the last {{< spell 191034 "Starfall" >}} with Drift so that it will be up during the last 8s of your cooldowns.
- Refresh {{< spell 8921 "Moonfire" >}} on up to 6 (12 with {{< spell 281847 "Twin Moons" >}}) targets when they will live for another ~20 seconds.
- https://wago.io/mYVIsyQN8 for filler. The recommendation this WeakAura gives is not correct when your targets will die before your cooldowns end or the targets are spread.
- If the filler is {{< spell 190984 "Wrath" >}} or up to 5 targets use {{< spell 78674 "Starsurge" >}} to prevent overcapping.

**Notes:**

- This should be used as a priority, going from top to bottom.


<div id="st">

## [What is my Single Target rotation?](#st)

</div>

The venthyr only version can be found [here](/balance/2021-06-05-Venthyr-Compendium/#single-target).

**Venthyr specific notes will be marked with (V) at the start of a point and Night Fae specific ones will be marked with (NF)**


**Single target priority list OUTSIDE cooldowns:** 
- Keep up {{< spell 8921 "Moonfire" >}}, {{< spell 93402 "Sunfire" >}} and {{< spell 202347 "Stellar Flare" >}} and refresh within pandemic(30% of base duration).
- Enter the next Eclipse, preferring Solar Eclipse.
- Cast {{< spell 211545 "Fury of Elune" >}} if it will be up again for your next usage in CA/Inc.
- (NF) Cast {{< spell 274281 "Moons" >}} if you are in Lunar Eclipse or you are overcapping charges inside solar eclipse. If possible save charges for CA/INC.
- Cast {{< spell 78674 "Starsurge" >}} when you would overcap Astral Power before entering the next Eclipse. This usually equates to spending 3 Starsurges at the start like you did with BoAT but can vary. Don't spend if you need to move soon.
- Cast {{< spell 190984 "Wrath" >}} in Solar Eclipse.
- Cast {{< spell 194153 "Starfire" >}} in Lunar Eclipse.
- Cast dots if have nothing to cast while you are moving.

**(V) Single target priority list BEFORE cooldowns:**
- Make sure to have 90+ Astral Power before using cooldowns. The only exception is when Bloodlust would run out before Inc expires at which point you Inc+Frenzy sooner. This happens with Bloodlust on pull.
- Make sure {{< spell 211545 "Fury of Elune" >}} will be up in the last 4 sec of your {{< spell 323546 "Ravenous Frenzy" >}}.

**(V) Single target priority list INSIDE cooldowns:**
Before the 5s extension buff:
- Use Berserking at the start of Frenzy without Bloodlust or at 6s of the initial buff remaining with Bloodlust.
- Use your trinket so that it will be for the rest of your cooldowns. Never ever use off gcd items/spells between casts, always use them during a gcd. For exact timings see [Timings sections](/balance/2021-06-05-Venthyr-Compendium/#timings).
- Use pot at 17s {{< spell 323546 "Ravenous Frenzy" >}} remaining
- Cast {{< spell 211545 "Fury of Elune" >}} if the initial {{< spell 323546 "Ravenous Frenzy" >}} has 4 or less seconds remaining
- Cast {{< spell 78674 "Starsurge" >}} to prevent capping Astral Power
- Keep up {{< spell 8921 "Moonfire" >}}, {{< spell 93402 "Sunfire" >}} and {{< spell 202347 "Stellar Flare" >}}
- Cast {{< spell 190984 "Wrath" >}} to fill until 150% haste at which point you should fill with {{< spell 194153 "Starfire" >}}.

**(V) During the 5s Ravenous Frenzy extension buff:**
- Cast {{< spell 78674 "Starsurge" >}} to spend all your Astral Power.
- Cast {{< spell 190984 "Wrath" >}} to fill.

**(NF)Convoke the Spirits and Pulsar usage:**
- Cast Convoke inside any {{< spell 194223 "CA" >}} / {{< spell 102560 "INC" >}} window (also meaing pulsar windows).
- If possible try lining up a pooled up Pulsar with {{< spell 102560 "INC" >}}. It is important to note that if you are already in Inc, proccing pulsar will extend the duration of Inc, but using Inc inside a pulsar window will not extend it.

**Notes:** 
- Due to no longer using Balance of All Things there is no longer as compelling of a reason to {{< spell 78674 "Starsurge" >}} at the beginning of an Eclipse and thus you can often save Astral Power for movement without any relevant dps loss. {{< spell 78674 "Starsurge" >}} Empowerment exists but it is a very weak effect.

- (V) With {{< spell 202354 "Stellar Drift" >}} AND {{< spell 114107 "Soul of the Forest" >}} it is only a 1% dps loss to use Starfall on CD including during Frenzy so if there is any movement at all use Starfall when you happen to be attacking a single target with it talented. With {{< spell 102560 "Incarnation" >}} talented you should avoid using Starfalls during Frenzy as it is a much bigger loss but with {{< spell 202354 "Stellar Drift" >}} Starfall should still be used to avoid downtime. Do not just use {{< spell 202354 "Stellar Drift" >}} for a pure single target fight as it is still a ~4% dps loss doing this compared to {{< spell 202347 "Stellar Flare " >}} unless there is no way of getting a good Frenzy window without it.


<div id="filler">
 
## [What is my filler priority inside CA?](#filler)

</div>

1 Target:
- Starfire if at or above 110% haste for Night Fae and 150% for Venthyr (You would currently need both Bloodlust and Power Infusion or other external haste buffs in order to reach this amount. A WeakAura tracking your current haste value might come in handy.)
- {{< spell 190984 "Wrath" >}} if below 110% haste for Night Fae and 150% for Venthyr

2 Targets and above:
- {{< spell 194153 "Starfire" >}}


<div id="owlkin-frenzy">

## [How do I use instant Starfire procs from Owlkin Frenzy?](#owlkin-frenzy)

</div>

When Lunar Eclipse is active use {{< spell 157228 "Owlkin Frenzy" >}} procs asap. When ONLY Solar Eclipse is active use it when fighting 3+ targets or when you need to move. Otherwise let it expire.


<div id="snapshot">

## [Do our dots snapshot?](#snapshot)

</div>

No, all of our periodic damage (like {{< spell 8921 "Moonfire" >}}, {{< spell 93402 "Sunfire" >}}, {{< spell 202347 "Stellar Flare " >}}) does NOT snapshot, everything is dynamic. That means any dots gain/lose the mastery bonus upon entering/leaving the Eclipse that buffs them and whenever any other stat/damage increases are applied/expire.


<div id="setup">

# [3. Flexible Setups:](#setup)

</div>


<div id="stats">
 
## [What is Balance Druids stat priority?](#stats)

</div>

Sim yourself using [Raidbots Top Gear](https://www.raidbots.com/simbot/topgear). Do not follow any stat priorities.


<div id="trinkets">

## [What Trinkets should I use?](#trinkets)

</div>

**DISCLAIMER: All of the trinkets in the following are examples. Your personal best trinkets depend on more factors such as ilvl meaning the best option is always to sim using either Top Gear, Droptimizer or Gear Compare.**

**There are 3 setups for trinket combinations:**
1. Double on-use (irrelevant in 9.2)
2. One on-use + one equip
3. Double equip


**Double on-use:**
This combination can prove to be the strongest from all the other trinket combinations IF you are playing **Venthyr with the {{< item 355315 "Sinful Hysteria" >}} legendary**. The only problem is that it requires specific trinkets and can be more difficult to use. You want to line up the last 5 sec from the IQD buff during Bloodlust AND Bell with the first 3 starsurges inside the Sinful Hysteria extension window.


Usable Trinkets:
- Slot 1: {{< item 179350 "Inscrutable Quantum Device" >}}
- Slot 2: {{< item 184842 "Instructor's Divine Bell" >}}


**2. One on-use, one equip:**
This combination should be used whenever double on-use is not a viable choice. A good example would be in M+ where Bell loses value due to it not scaling into AoE as well.

Usable trinkets:
- Slot 1 (Equip): {{< item 186421 "Forbidden Necromantic Tome" >}}, {{< item 178708 "Unbound Changeling" >}}, {{< item 186423 "Titanic Ocular Gland" >}} and others.
- Slot 2 (On-use): {{< item 179350 "Inscrutable Quantum Device" >}}, {{< item 180117 "Empyreal Ordnance" >}} and others. 


**3. Double Equip:**
Double equip items should never be played unless it can't be avoided (if for example you simply don't have any good on-use items) due to our CA/Inc being so much of our damage with any Covenant.

Usable trinkets:
- Slot 1+2 (Equip): {{< item 186423 "Titanic Ocular Gland" >}}, {{< item 186421 "Forbidden Necromantic Tome" >}}, {{< item 178708 "Unbound Changeling" >}}, {{< item 178386 "Insignia of Alacrity" >}} and others.

**Notable trinkets:**
{{< item 179350 "Inscrutable Quantum Device" >}}: This trinket has the potential to be the best on-use trinket by a large margin if the conditions found in [#11](#iqd) are met. These ultimately mean that the trinket is extremely good in M+ and whenever you can gurantee that later trinket usages are either in Bloodlust or when healers still have enough mana. You can adjust the value in sims using the IQD Stat Proc Chance option which will set the chance the trinket gives stats outside Bloodlust.

{{< item 184842 "Instructor's Divine Bell" >}}: Unlike the Quantum Device, the bell is a very consistent trinket that gives us a lot of mastery inside our burst windows. You can farm it by switching between a maxed Covenant and a Covenant without any progress in the mission table which will infinitely reset missions until you get the bell.

{{< item 180117 "Empyreal Ordnance" >}}: A pretty unique trinket that is split into two parts: a dot and a buff. After the dot finishes, the buff part of the trinket comes back to the caster. Due to this trinket putting other on use trinkets on a 40 sec cd, it should only be used with an equip trinket. If IQD is not usable or the ilvl discrepancy between these two trinkets is too big, then this trinket might be the best choice as Venthyr.

{{< item 186421 "Forbidden Necromantic Tome" >}}: An overall solid trinket that can be obtained at higher ilvl than other trinkets.

{{< item 186423 "Titanic Ocular Gland" >}}: A very good trinket if you are able above 50% health most of the encounter (which should essentially be all of them).

{{< item 178708 "Unbound Changeling" >}}: This trinket gains most of its value from the fact that it is convertable into a stat proc of your choice by eating the corresponding food. Once a day it has a chance to proc 3 secondary stats which further increases its value. Mastery proc can be used a default but sim to find which secondary it should proc.

{{< item 178809 "Soulletting Ruby" >}}: Although this trinket gives crit it gives a very high amount of it making it a decent option for Night Fae if you don't have access to another on-use trinket. When using it mind that it has a short delay before getting the buff depending on distance to the target.


<div id="talents">
 
## [What Talents should I run?](#talents)

</div>

**Default single target setup (pure single target raid bosses):**
{{< talents spec="balance" src="live" recommend="311,123,133,223,123,113,233" >}}
{{< spell 211545 "Fury of Elune" >}} and {{< spell 102560 "Incarnation" >}} should be used as Venthyr. {{< spell 274281 "New Moon" >}} should be picked for any other covenant.

**Default AoE setup (M+ and heavy AoE bosses):**
{{< talents spec="balance" src="live" recommend="332,113,133,223,311,331,231" >}}
Note that {{< spell 248280 "Force of Nature" >}} can and should be used in M+ for any key level where the tank could die even though they are a minor dps loss.
WoE performs better on 4+ sustained targets or heavy AoE burst.(2+ targets in 9.2)
The choice between {{< spell 281847 "Twin Moons" >}} and Drift depends on how long targets live and how much value the movement has. A general rule of thumb is pick {{< spell 281847 "Twin Moons" >}} if there are consistently 6+ targets that live 20+ seconds. (This ammount gets lower in 9.2)

**Mixed target count or mostly spread AoE (Council type bosses or bosses with add waves):**
{{< talents spec="balance" src="live" recommend="321,113,133,223,213,231,232" >}}
{{< spell 114107 "Soul of the forest" >}} should only be picked for bosses with extended stacked AoE.


<div id="t50">
 
## [T50 row choices and playstyle (9.1)](#t50)

<div>
 

**The currently most viable playstyles are:**

   - Venthyr Hysteria
   - NF Pulsar 
   - Kyrian Kindred Affinity

**Venthyr Hysteria:**

- {{< spell 343647 "Solstice" >}} is playable in spread aoe but requires 3+ targets of permanent uptime which can be very very hard to find. The closest example where Solstice would beat FoE on paper would be Council of Blood from Castle Nathria but none of the current raid.

- {{< spell 202770 "FoE" >}} is incredibly strong with this build beating out any other talent in 99% of the situations on both ST and stacked AoE. You will want to use FoE whenever you have 4 sec left on Ravenous Frenzy inside Incarnation, and on cd inside any eclipse whenever outside of it.

- {{< spell 274281 "Moons" >}} should never get picked with this build as they are inferior to FoE in every scenario.

**Night Fae Pulsar + Kyrian KA:**

- {{< spell 343647 "Solstice" >}} is a better choice for this build when compared to Venthyr because of the fact that FoE is not as strong, meaning that you will have more oportunities to pick this talent depending on the raid fight.

- {{< spell 202770 "FoE" >}} is again very strong, but this time only on stacked AOE rather than ST and should be used when you enter CA or on cd as the first global of a new eclipse if CA+Convoke are not available. 

- {{< spell 274281 "Moons" >}} should be picked over FoE as they are the roughly a 0.7% dps upgrade over FoE on pure ST. Save moons for CA/Inc without overcapping and if not inside CA/Inc they should preferably be casted inside Lunar Eclipse.


<div id="conduits">
 
## [What Conduits should I pick?](#conduits)

</div>

**Potency:**
- {{< spell 341383 "Endless Thrist" >}}: 100% of the time this should be your first go to potency slot as Venthyr.
- {{< spell 341446 "Conflux of the Elements" >}}: 100% of the time this should be your first go to potency slot as Night Fae.
- {{< spell 341378 "Deep Allegiance" >}}: 90% of the time this should be your first go to potency slot as Kyrian as it enables 45sec bond.
- {{< spell 340708 "Fury of the Skies" >}}: Default go to as a secondary slot.
- {{< spell 340706 "Precise Alignment" >}}: For Venthyr this is an exceptionally good conduit because of the Sinful Hysteria legendary and should always be used in tandem with it (in 9.1.5). For Pulsar in general this is the 3rd strongest conduit. Without Pulsar it has the same value as Umbral.
- {{< spell 340719 "Umbral Intensity" >}}: Situational usage, but gets outshone by Fury and Precise. On par with Stellar Inspiration for 4th slot. (in 9.2)
- {{< spell 340720 "Stellar Inspiration" >}}: On par or even a bit better than Umbral on sustained AoE. (in 9.2)

Notes: 
  - This should be used as a priority list, going from top to bottom.
  - {{< spell 340706 "Precise Alignment" >}} is a must have as Venthyr in 9.1.5.


**Endurance:**
- {{< spell 340553 "Well-Honed Instincts" >}}: A must have. One of the most overtuned endurance conduits in the game raid wise.
- {{< spell 340540 "Ursine Vigor" >}}: Really good if you will ever go into bear form to soak an ability. Especially good on progression and if you will ever press Heart of the Wild while being talented into Guardian Affinity.
- {{< spell 340529 "Tough as Bark" >}}: Good if you press Barkskin a lot or the fight timers allow a shorter Barkskin to line up better with certain abilities.
- {{< spell 357888 "Condensed Anima Sphere" >}}: Probably the best pick all around if you are not targeting a specific conduit for a specific fight or if you have a spot open and do not know what else to go for.
- {{< spell 340543 "Innate Resolve" >}}: Mediocre value since it will only have value when {{< spell 340553 "Well-Honed Instincts" >}} procs or you are already actively healing yourself. In both cases you are very likely already safe.
- {{< spell 340605 "Layered Mane" >}}: Unlike Well-Honed Instincs this is a Guardian conduit that actually only Guardian wants.

Notes: Default Instincts and fill in the rest as needed.

**Finesse:**
- {{< spell 341450 "Front of the Pack" >}}: The best default pick as roar is very useful in many raid encounters and to get around dungeons quicker.
- {{< spell 341280 "Born Anew" >}}: Useful pick to get someone up again without them losing as much damage from the lost food buff. Can no longer be used before a pull as the food buff will reset to 20 main stat on raid combat start.
- {{< spell 341451 "Born of the Wilds" >}}: Good in M+ if you have to offheal a lot through Heart of the Wild.
- {{< spell 340545 "Tireless Pursuit" >}}: Can be very strong if you often find yourself using Cat Form/Travel Form to dodge mechanics/get around.


<div id="soulbinds">
 
## [What Soulbinds should I pick?](#soulbinds)

</div>

**Night Fae:**
- 99% of the time [Niya](https://www.wowhead.com/soulbind-calc/night-fae/niya/druid/AwCW6r4TBTXGCBUy5AglMuII) - Use {{< spell 320659 "Burrs" >}} for 1-3 targets and when there aren't any immune targets it can proc on. Otherwise use a second/third potency conduit.
- 1% of the time [Korayn](https://www.wowhead.com/soulbind-calc/night-fae/korayn/druid/AwCW6r4RBTXGCA) - good when the 25% crit on hitting a new target Soulbind can abused.

**Venthyr:**
- By default [Theotar](https://www.wowhead.com/soulbind-calc/venthyr/theotar-the-mad-duke/druid/AwCW75YCFTUgACU1ygASBTWHACUy4gAiBTJJABUyPwA) with Wasteland Propriety.
- Whenever you can time your CDs to line up with Euphoria and it is not viable to stand in the Umbrella [Nadja](https://www.wowhead.com/soulbind-calc/venthyr/nadjia-the-mistblade/druid/AwCWr5YDBTUgABU1ywAlNcoAEgUy4gAlNYcAIRUySQA) with Dauntless Duelist for ST and a 3rd potency slot for AOE. This Soulbind is generally not advised though.
  
**Kyrian:**
- By default [Mikanikos](https://www.wowhead.com/soulbind-calc/kyrian/forgelite-prime-mikanikos/druid/AwCW5ZYTBTWCCBUy5AglMuII).

<div id="potions">

## [What potions should I use?](#potions)

</div>

{{< spell 307162 "Potion of Spectral Intellect" >}} for all situations.



<div id="meaningfulchoice">

# [4.Meaningful Choices:](#meaningfulchoice)

</div>


<div id="legendaries">

## [What Legendaries should I craft?](#legendaries)

</div>

**Night Fae:**

{{< spell 338668 "Pulsar" >}} with Mastery + Haste/Vers

**Venthyr:**

{{< spell 355315 "Sinful Hysteria" >}} with Mastery + Haste

**Kyrian:**

{{< spell 354115 "Kindred Affinity" >}} with Mastery + Haste
 
**9.2 Double Legendary:**  
  
 {{< spell 338668 "Pulsar" >}} + Covenant Legendary with Mastery + Haste.
  
<div id="legendaries-slot">

## [What slot do I craft legendaries in?](#legendaries-slot)

</div>

**{{< spell 354109 "Sinful Hysteria" >}} slot:**

Craft this on Belt because of the Domination Sockets.

**{{< spell 338668 "Pulsar" >}} slot:**

Craft this on Ring because of the Domination Sockets.

**{{< spell 338657 "Circle" >}} slot:**

Ring because of the Domination Sockets.

**{{< spell 339942 "BoAT" >}} slot:**

You should craft the legendary on Legs because of the Domination Sockets.

<div id="covenant">

## [What Covenant should I pick?](#covenant)

</div>
  
**Venthyr:**
9.1.5: Currently with the legendary {{< item 355315 "Sinful Hysteria" >}} it outperforms Night Fae in both Single target and AOE and should be your default pick when mainly playing Balance Druid.
  
<br>9.2: In 9.2 Venthyr will still be the best covenant if the NF utility or damage profile is not needed. It is worth noting that the difference between NF and Venthyr is now much closer due to the Hysteria nerf and the new tier set.

**Night Fae:**

9.1.5: Night Fae Balance druid is still a viable spec and should be your default pick when playing multiple Druid specs or when you just prefer the aesthetics or gameplay.
  
<br>9.2: With the new tier set, Night Fae will be much closer to Venthyr ST dps wise and should be picked depending on encounter.


**Kyrian:**

9.1.5: Can be competitive with the Kyrian legendary due the legendary's absurd power but is a fair amount behind when not including it.
  
<br>9.2: With the nerf to the Kyrian legendary, this covenant is now on par with venthyr on raid dps. Because of how clunky the actual bond is and how fast you can lose value on it you should always try to use the other two viable covenants.

**Necrolord:**

9.1.5: Not currently competitive.
  
<br>9.2: Still not competitive.
 
**Notes:**
For more 9.2 information refer to [the news](#news).

<div id="domination-sockets">

## [What Domination Sockets should I use?](#domination-sockets)

</div>

With the current iteration of Domination Sockets you should use the Chaos Bane (Unholy) set. After you get the set which includes the Dyz gem, you should look to get the Bek, Cor and Kyr gems which are all situationally extremely strong. In add fights prefer the Cor gem, in single target fights prefer the Bek gem (other than Sylvanas) and in all fights that require more sustain or you need a 5th socket if either Bek or Cor are not giving any significant value, use Kyr.
  

  
<div id="covenants">

# [5. Covenant specific tips:](#covenants)

</div>


<div id="nightfae">

## [Night Fae:](#nightfae)

</div>

**Should I delay Convoke for it to line up with CA?**


Yes you should always delay {{< spell 323764 "Convoke" >}} UNLESS you can cast a Convoke without losing a {{< spell 194223 "CA" >}}+Convoke (both at the same time) cast. This will for example happen in 5 minute fights where you would cast Convoke+CA on pull, Convoke alone after 2 minutes and then Convoke+CA at 4 minutes.

For M+ the same logic applies when you for example know you won't be using your CA for another 2min due to saving it for a boss you can use a solo Convoke. This should be minimized though as every desynced Convoke is a damage loss.

If you are playing with the Primordial Arcanic Pulsar legendary you should use {{< spell 323764 "Convoke" >}} whenever you are in either a Pulsar or a {{< spell 194223 "CA" >}} / {{< spell 102560 "INC" >}} window.
  
**What is the chance of getting Full Moon during Convoke?**
  
The chance of getting a Full Moon during Convoke the Spirits is based on a "Stacked Deck" system with a deck of 5 cards. What this means every time we enter a new combat we get a deck of 5 cards and one of them is Full Moon. Every time we use Convoke one card is drawn so the first cast always has a 20% chance of casting Full Moon. If the first cast didn't proc a Full Moon the second cast will have a 1/4=25% chance to proc one and so on. After the whole deck has been drawn or you leave combat a new deck of 5 cards is created. In a normal raid encounter this mechanic means that you will never get more than 1 Full Moon unless you died as you'd have to cast 6 Convokes to even have a chance to get another Full Moon.

**How does the covenant legendary affect Convoke?**

Currently it reduces the spells cast by 1/4 and casts 2.4 Wraths, 2.2 Starsurges, 0.9 Starfalls and 0.425 Full Moons on average when every target is dotted. This is about half the Wrath and Starsurge casts than without the legendary. Addtionally the legendary reduces the amount of cards in the deck for Full Moon from 5 to 2 but gives the Full Moon card only a 85% chance to proc the Full Moon.

<div id="venthyr">

## [Venthyr:](#venthyr)

</div>

[The Venthyr Compendium can be found here.](/balance/2021-06-05-Venthyr-Compendium)

<div id="minmax">

# [MinMax:](#minmax)
  
</div>

The following are super minor things you can do to gain a small amount of extra damage once you are comfortable with the rotation:
- Dotting outside Eclipse without losing dot uptime on single target is a ~0.4% gain when not using Solstice.
- At 150%+ haste using {{< spell 194153 "Starfire" >}} is minorly better than {{< spell 190984 "Wrath" >}} on single target. This will only happen with Power Infusion or very high base haste.
- When {{< spell 323546 "Ravenous Frenzy" >}} has less than your current fillers cast time left you should already start dumping Astral Power to get another 1-2 stacks. This is about a 0.6% gain.
- With {{< spell 202354 "Stellar Drift" >}} it is only a very minor loss (1-2%) to {{< spell 191034 "Starfall" >}} during {{< spell 323546 "Ravenous Frenzy" >}} as long as you enter Sinful Hysteria with 90+ AsP.
- Without Incarnation and a low enough {{< spell 340706 "Precise Alignment" >}} it is a minor gain to use {{< spell 323546 "Ravenous Frenzy" >}}  before Celestial Alignment so that CA will be up throughout Frenzy+Hysteria. The exact timing depends on your {{< spell 340706 "Precise Alignment" >}} rank but it should be no more than 2 globals after the Frenzy cast.
- If the fight time allows it wait for Euphoria/Fatal Flaw(Nadija Soulbinds) before using cooldowns. This is relevant for 5-6 min kill times.
- If the fight allows it wait for pot to be up again. This is relevant for 6min fights.

<div id="gear">

# [Gear:](#gear)
  
</div>

**Simming:**

Once everything is on live you will be able to sim as normal and that will, as always, give you the best results. It is to note that for Venthyr sims adjusting the fight duration can have a relevant impact on how strong some items may be so it can be beneficial to adjust the sim duration to fight the fight you are simming for. Keep in mind that there will be a 20% fight length variance in sims meaning that a 5min sim is actually a 4-6min sim.

**Trinkets:**

Generally you will want an on-use trinket and the strongest passive trinket you can find. The strongest on-use trinkets are {{< item 179350 "Inscrutable Quantum Device" >}}, {{< item 180117 "Empyreal Ordnance" >}} (yes, without double on-use) and {{< item 184842 "Instructor's Divine Bell" >}} (yes, it's still broken even at low ilvl). IQD and Bell can be combined for a minor dps increase in the sub 0.5% area, although if that is better with your ilvl trinket you will have to sim. The raid on-use trinkets are all bad because we are a 3min class unless you cannot have your stats be mastery>haste for IQD.

As a passive trinket you have a plethora of options. For single target your best options are the new trinkets {{< item 186423 "Titanic Ocular Gland" >}} (2nd boss raid), {{< item 186421 "Forbidden Necromantic Tome" >}} (last boss raid), {{< item 186422 "Tome of Monstrous Constructions" >}} (1st boss raid), {{< item 178769 "Infinitely Divisble Ooze" >}}, {{< item 178708 "Unbound Changeling" >}}, {{< item 187447 "Soul Cage Fragment" >}} (World Boss) and a bunch of others. For AoE/M+ the damage proc trinkets fall off meaning you won't want the Tome or Oooze but the other trinkets stay as good. As always just sim what trinkets are best from the ones you have.

**Ideal stats:**

Ideal stats are something that are not realistic to achieve and should thus not be a goal of any kind, this section is purely for interest. Independent of that with Venthyr Balance Druid mastery and haste are far, far more valuable than crit and vers as your sims will show. In fact when you could choose any kind of stats you wouldn't want any crit or vers but again this is not realistic.


<div id="kyrian">

## [Kyrian:](#kyrian)

</div>


- How does Kindred Spirits (Kyrian covenant ability) work?

When you use {{< spell 326434 "Kindred Spirits" >}} both people get an empty pool that lasts 20 seconds and 15% of your damage, healing and damage taken empties the pool to increase/absorb each. Each person also gets a buff that lasts 10 seconds and during that time 20% of your damage fills up the pool of the other person.



- Who do I bond Kindred Spirits with and when do I use it?

With {{< spell 354115 "Kindred Affinity" >}} you prefer to bond with a Night Fae because of the haste. Kyrian sadly gives very poor value and should be avoided.
An experimental sheet for Kindred Affinity in 9.2 with tier sets and 2 legendaries and more information can be found [here](https://docs.google.com/spreadsheets/d/1baQypWt2RjCYvtRQ7T5fPXqK18FeZON9XtR-LRvSGXo/edit?usp=sharing).


<div id="Miscellaneous">

# [6. Miscellaneous:](#Miscellaneous)

</div>

<div id="swifty-macro">

## [Useful CA + Convoke + Trinket macro:](#swifty-macro)

</div>


```
#showtooltip
/stopmacro [channeling: convoke the spirits]
/stopmacro [noform:4]
/cast Celestial Alignment
/cleartarget
/use 13
/targetlasttarget
/use Potion of Spectral Intellect
/cast Convoke the Spirits
/cqs
```

**Explanation:**

- This is for Night Fae only!
- DO NOT use this macro while on the gcd (like just having casted a dot or Starsurge) or the {{< spell 323764 "Convoke" >}} will not fire. Wait until the gcd is finished.

- "#showtooltip" makes the tooltip of {{< spell 194223 "CA" >}} show upon hovering over the macro.
- "/stopmacro [channeling: convoke the spirits]" prevents the macro from being casted if you are currently channeling {{< spell 323764 "Convoke" >}}.
- "/stopmacro [noform:4]" prevents the macro from being casted if you are NOT in Moonkin Form.
- "/cast Celestial Alignment" casts {{< spell 194223 "CA" >}}.
- "/cleartarget" clears your current target. This is useful whenever using the "Inscrutable Quantum Device" trinket and makes it so that the trinket does not use its execute part. Do not use this with a targeted trinket.
- "/use 13" uses the trinket in the 13/upper slot. You can use 14 if your on-use trinket is in the bottom slot.
- "/targetlasttarget retargets your last target after being cleared by the "cleartarget". 
- "/use Potion of Spectral Intellect" uses your potion. If your potion is not assigned to any specific point you can put it here.
- "/cast Convoke the Spirits" uses the Nightfae covenant ability.
- "/cqs" cancels your queued spell. Convoke can sometimes cancel itself when using a macro due to weirdness with spell queuing. This stops any weirdness thus your Convoke from ever cancelling itself.

You can and should remove/add other commands to this macro depending on situation. For example the potion line, or the "stopmacro [noform:4]" line.


<div id="iqd">
 
## [How does Inscrutable Quantum Device work?](#iqd)

</div>

When this trinket is used, it triggers the effect with the first condition that applies from the following list:

- Remove CC from self: Always triggers if you are under a hard CC mechanic, does not trigger if the CC mechanic does not prevent the player from acting (e.g., it won't trigger while rooted).

- Heal spell: Triggers on self or a nearby target with less than 30% health remaining.

- Execute damage: Deals damage to the target if it is an enemy with less than 20% health remaining. (You can prevent this by untargetting the mob via a macro, see [#19](#swifty-macro).)

- Secondary stat buff with Bloodlust: If a Bloodlust buff is up, the stat buff will last 25s instead of the default 20s, always be your highest rating and have higher prio than giving mana.

- Mana: Gives mana to a healer with less than 30% mana.

- Secondary stat buff: Grants a 20s secondary stat buff randomly selected from the player's two highest secondary stats in terms of rating.

**Notes:**
  
  - If you have a dead tank in your group the IQD will force proc an npc that is supposed to taunt the boss. (does not do anything in practice)
  
  - If your healers are below 30% mana, you can outrange them (40y range) and force it not to proc. 
  
  
<div id="astral-damage">
 
## [What is Astral damage?](#astral-damage)

</div>

Astral damage is Arcane and Nature damage at the same time meaning that these spells benefit from effects that buff either spell school and double dip whenever effects that buff both are active. Mind that class buffs only affect class spells so if a trinket does nature or arcane damage they are not affected by our buffs to these spell classes.
  
  
<div id="M+">

# [7. Mythic+:](#M+)

</div>
  
<div id="low-dmg">
 
## [Why am I doing low damage?](#low-dmg)

<div>


This is obviously a very hard question to answer correctly without a LOT of context, but nonetheless it is probably one of the most asked questions. 
Some conditionals for doing high damage as a balance druids are:
  
**Key level**
<br>The higher the key level the more you will be able to apply your dots and ramp your damage.

  **Your group composition and how to approach playing around it**
<br>A good example for this would be you doing a weekly +15 key with your venthyr moonkin friend. In a scenario like this you would want to desync your cooldowns. Most of the time, especially as a venthyr druid in lower to medium keys, you want your cooldowns to be uncontested by other people in your group, meaning that you are the only person that is using cooldowns on a pack.
  
**Your gear**
<br>Obviously, like anything else in WoW, your gear will matter no matter what. The better the gear, the more damage you will do. That being said a big trap would be chasing gear over improving personal play. You can get away with using [topgear](https://www.raidbots.com/simbot/topgear) and [Droptimiser](https://www.raidbots.com/simbot/droptimiser) until you reach the very high echelons of raiding or M+.

**Route and Pulls**
<br>Especially as a Venthyr it is imperative that your tank pulls around your cooldowns, as most of your damage comes from those windows. If you have to use your cooldowns on a 3 mob pack that lasts 15 seconds you will want to Hearthstone right out of the key. 

**Your own skill**
<br>Obviously above all else pressing your buttons correctly will net you the most damage. Refer to the [aoe priority](#aoe) for more information.


<div id="M+Talents">
 
## [M+ Talents](#M+Talents)

<div>
{{< talents spec="balance" src="live" recommend="223,213,123,333,311,331,131" >}}
 
<div id="M+Soulbinds">
 
## [M+ Soulbinds](#M+Soulbinds)

<div>

<br>[Venthyr](https://www.wowhead.com/soulbind-calc/venthyr/theotar-the-mad-duke/druid/AwCWb74BFTUgCBIFNYcIJTLiCCMFMkkIFXYACDUyMQg)
<br>[Night Fae](https://www.wowhead.com/soulbind-calc/night-fae/niya/druid/AwCW5b4CBTXKCCU1IAgTBTXGCBUy5AglMuIIIhUySQgldgAI)
 
<div id="M+Sockets">
 
## [M+ Domination Sockets](#M+Sockets)

<div>
 
Cor>Dyz=Bek=Kyr>Rev=Jas
 
 
 
<div id="M+Anima">
 
## [M+ Anima Powers](#M+Anima)

<div>

Soggodon the Breaker 	
<br> -	Stone Ward

Incinerator Arkolath 	
<br> -  Champion’s Brand
<br> -  Bolstering (only in explosive week)
 
Oros Coldheart 		
<br> -	Regenerative Fungus
 
Executioner Varruth
<br> - Volcanic Plumage (for pack control if needed as a triple pick for stability)
<br> - Dagger of Necrotic Wounding (tyran/low pack density dung)
<br> - Champion’s Brand (rest) 
 
<div id="M+Improve">
 
## [How to Improve in M+](#M+Improve)

<div>

If you want to push to the next level you can improve a lot by recording your gameplay. Afterwards, review the recordings while looking out for either small micro errors in your gameplay like optimization on dotting, {{< spell 191034 "Starfall" >}} uptime, Eclipse cycling and {{< spell 197911 "AP" >}} pooling. Be on the lookout for improvements on what trash packs to pull and how they are controlled. 
 Some macro tips to look out for may include but are not limited to:
- Offhealing when necessary in order to save or stabilize a pull. 
- Setting up future packs if a double pull is incoming or you are trying to skip a pack. This can be done by locking a whole pack in place by rooting/hibernating the “leader” of the pack. Most patrol packs are following one certain mob in that pack, usually the biggest mob or the one in the front. (Ether Divers in SoA)
- Utilising {{< spell 29166 "Innervate" >}} preemptively in order for your group to be able to chain more packs and not have to wait for mana.
- Pooling AP as a pack is dying in order to be above 50AP before the next group of mobs to be able to maintain {{< spell 191034 "Starfall" >}} from the start.
 
 
 ## [M+ Covenants by Luddeus](#M+covenants)
 
If trash dies too fast, Moonkin just doesn't do any damage. This is more of a Moonkin issue than a Venthyr vs Night Fae issue. Yes, the problem is a tad more exacerbated from Venthyr since they don't do much damage out of CDs. Night Fae still technically has pulsar for some trash damage, but this doesn't really matter at all. You're not going to be doing decent damage on trash as a boomkin if things die fast, and besides, it doesn't matter. Things dying fast is good, it means the key is getting timed and that's all that matters. Overall dps is a horrible metric to look at by itself. 
  
Venthyr will do much better than Night Fae in more relevant keys where trash stays alive. A key in which Venthyr does worse than Night Fae, in general, is very likely a key where it doesn’t really matter what covenant you are since you're gonna be timing the key. This doesn't just depend on one single metric. It's a combination of key level, the dungeon, how much the tank pulls, your group's gear/dmg, etc. There isn't any set goal where you can say "Oh, Venthyr is better above X level", or "Oh, Venthyr is only good when group is pulling around my CDs". These statements are all incorrect by themselves, and should not be parroted.
Keep in mind these suggestions are assuming you only care about PvE as Moonkin. If you regularly play feral and resto in relevant content, Night Fae might be the better choice for you.

  
<div id="Utility">

# [8. Utility:](#Utility)

</div>
  
  
## Balance Druid Utility:

{{< spell 29166 "Innervate" >}} - Healer no mana costs for 10sec - use on yulon monk > disc > everything else (also works with Resto Aff HotW)

{{< spell 22812 "Barkskin" >}} - 20% DR on 60sec CD (reduced by {{< spell 340529 "Tough as Bark" >}} and {{< spell 265144 "Symbol of Hope" >}}), usable while stunned, frozen, incapacitated, feared or asleep. Also prevents your casts from being pushed back.

{{< spell 61391 "Typhoon" >}} - AoE Knockback on 30s CD, can be used for purely displacing, interrupting or in tandem with Ursol's Vortex (read below). Keep in mind that knockbacks also have DR.

{{< spell 33786 "Cyclone" >}} - Stasis/Banish on enemy for 6sec, 25y. Can be used if an add needs to not die (bolstering)

{{< spell 2908 "Soothe" >}} - Enrage dispell on an enemy, 10s CD (CD incurs even if nothing is dispelled)

{{< spell 2782 "Remove Corruption" >}} - Curse and Poison dispell on a friendly Target, 8s CD (CD does not incur if nothing is dispelled)

{{< spell 339 "Entangling Roots" >}} - 30sec snare, 40y range - can affect only one target (independent of mass entanglement)

{{< spell 2637 "Hibernate" >}} - 40sec Sleep/Incapacitate on enemy Beasts and Dragonkins, 35y (can also be used to interrupt casts)

{{< spell 106898 "Stampeding Roar" >}} - Raid wide movement speed increase (60%) for 8 sec (range and duration increased with conduit). Force shifts into Bear form if not in either Bear Form or Cat Form. If you force shift into bear form the ability incurs a longer GCD.

**Affinities:**

{{< spell 197492 "Restoration Affinity" >}}: unlocks {{< spell 145109 "Ysera's Gift" >}}, {{< spell 102793 "Ursol's Vortex" >}}, {{< spell 48438 "Wild Growth" >}}, {{< spell 18562 "Swiftmend" >}}, {{< spell 774 "Rejuvenation" >}}

{{< spell 197491 "Guardian Affinity" >}}: unlocks {{< spell 16931 "Thick Hide" >}}, {{< spell 99 "Incapacitating Roar" >}}, {{< spell 33917 "Mangle" >}}, {{< spell 192081 "Ironfur" >}}, {{< spell 22842 "Frenzied Regeneration" >}}

{{< spell 197490 "Feral Affinity" >}} : unlocks {{< spell 131768 "Feline Swiftness" >}} and {{< spell 22570 "Maim" >}} (the only reasons you would pick feral aff)

{{< spell 1850 "Dash" >}} - Self 60% movement speed increase while in Cat Form 10s duration. (force shifts into cat form)

{{< spell 99 "Incapacitating Roar" >}} - 3 sec aoe Incapacitate, 30s CD - mainly used to interrupt unkickable casts or channels

{{< spell 102793 "Ursol's Vortex" >}} - AoE 50% Slow + grips mobs inside it if they try to leave (once), 60s CD - mainly used for tank kiting, can be used in tandem with Typhoon to create a budget gorefiend's grasp

{{< spell 22570 "Maim" >}} - Stun based on how many CPs you have (1sec per CP) - not used in 99.999% of cases

**Nature's Control:**

{{< spell 5211 "Mighty Bash" >}} - Melee range 4s stun usable in any form, 60s CD

{{< spell 102359 "Mass Entanglement" >}} - 30s Root that aoes based off of your target (you can have both entangling roots and mass entangle at the same time), 30s CD

{{< spell 108291 "Heart of the Wild" >}} - Grants a specific buff depending on your affinity
  + {{< spell 108293 "Guardian" >}} - 20% stam, 2 frenzied regens, ironfur stackable - force shifts into bear form, buff only while in bear form (45% stam, 220% armor total + frenzied)
  + {{< spell 108294 "Restoration" >}} - healing increased by 30% mana cost reduction by 50% - can use innervate on yourself
  + {{< spell 108292 "Feral" >}} - never use this

{{< spell 8936 "Regrowth" >}} - direct heal + hot, castable in Moonkin Form

{{< spell 774 "Rejuvenation" >}} - hot (instant) 12s dur, force shifts into Human Form

{{< spell 48438 "Wild Growth" >}} - aoe hot (ramps down, 30k ish healing per cast), force shifts into Human Form

{{< spell 18562 "Swiftmend" >}} - very big heal that consumes a hot, force shifts into Human Form (try to use when the HoT has low duration esp off regrowths or ramped down wild growths)

{{< spell 22842 "Frenzied Regeneration" >}} - 24% max HP heal over time. If you leave Bear form the effect disappears. 

{{< spell 3025 "Cat Form" >}} - Stance, 30% movement speed, going into or out of cat form removes slows and roots.

{{< spell 783 "Travel Form" >}} - Stance, 40% movement speed while in combat, 100% movement speed while out of combat, going into or out of travel form removes slows and roots.

{{< spell 5487 "Bear Form" >}} - Stance, 25% stamina 220% armor, stamina can be used to tank mechanics since you will be losing a smaller % of hp inside it leaving you with higher hp when you go out of it. Going into or out of bear form removes slows and roots.

{{< spell 164862 "Flap" >}} - Slow fall effect that has to be channeled. Keeps velocity, costs 1 GCD. Can be used after Wild Charge to extend the jump and travel more distance.

{{< spell 102401 "Wild Charge" >}} - 15s CD, off GCD 
  + Moonkin - Disengage / bound backwards away from current location - can be extended by jumping before and/or using Flap after it.
  + Human - Fly to an ally's position - can be used on a separare keybind with a cancelform mouseover wild charge macro.
  + Cat - Leaps behind an enemy target and slows it.
  + Bear - Charges to your target and briefly rooting it.
  + Travel - leap forward (longer than moonkin form)

{{< spell 37846 "Force of Nature" >}} - Taunts everything in a radius near the initial placement of the trees. 60s CD. The trees will start targeting whatever your target was upon placing them. 

{{< spell 78675 "Solar Beam" >}} - ST interrupt on main target with 6s lockout that places an aoe silence ring on the ground. The silence ring does not work on some mobs but the actual interrupt does, be careful with this.
