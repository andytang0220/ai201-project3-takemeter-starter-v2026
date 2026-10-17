# TakeMeter

> ### 👋 Start here
>
> **New to this repo? Read [RUNNING.md](RUNNING.md) first** — setup, the
> notebook, the baseline, and what to do when something breaks.
>
> Once `python test.py` passes:
>
> ```bash
> head -5 data/practice_labels.csv     # the shape your labels.csv needs
> ```
>
> Then open `takemeter.ipynb` **in this folder** — in VS Code, or with
> `jupyter notebook` if you prefer. Pick the kernel: the `.venv` inside this
> project. Run section 1, which reports the hardware you'll be training on.
> Everything else waits until you have data.
>
> Nothing to upload, nothing to connect, no accounts and no keys. The notebook
> runs on your machine and writes next to your code.
>
> **The rest of this file is your submission.** Fill it in as you go.

---

<!-- ─────────────────────────────────────────────────────────────────────────
     HOW TO USE THIS FILE

     Unit 5 asks for the first five sections. Unit 6 adds the five below them.

     Everything is pasted as TEXT. No screenshots, no images.

     ⚠️ The confusion matrix especially. The notebook prints one as a markdown
     table, ready to copy. A screenshot of a matrix earns nothing. Paste the
     table.
     ───────────────────────────────────────────────────────────────────────── -->

<!-- ═══════════════════════ UNIT 5 — THE BUILD ═══════════════════════ -->

## What This Does

<!-- Your community, and what your classifier sorts posts into. Three or four
     sentences. -->



---

## Label Taxonomy

<!-- Each label: a one-sentence definition and two real examples from your
     reading. Then your decision rule for the hardest boundary.

     The decision rule is worth a point on its own and it's the thing most
     people leave out. Every taxonomy has a hardest boundary. Name yours. -->

### `wish`

**Definition: Proposes a specific change but leaves how it works up to the reader. The core behavior is missing, offered as options or guesses (“maybe crafted from…?”), or the whole change is one clause.**

**Example 1: Have ice bricks & variants be slippery like packed ice**
>They're crafted directly from packed ice. I'd understand if there was, like, cobblestone mixed in, but it's just ice. Why do they not preserve the lower friction?

**Example 2: A new structure with mobs would be awesome in the snow biomes!**
>I’m silently holding out hope that this new drop will include an ice structure of some kind that spawns in snow biomes made from the ice bricks mixed with other blocks. Pillagers could spawn in this structure as an outpost-type structure and it would be a great way to bring in the Iceologer.
>The new snapshot promo from Minecraft’s Twitter has hyped me up with this idea. Give me your thoughts and opinions!

### `spec`

**Definition: Describes how the proposed thing works concretely enough that two readers would picture the same feature, but gives no reasoning beyond a motive.**

**Example 1: Ash blocks and lye**
>The idea is you burn a flammable block, and instead of disappearing it’s replaced with an ash block, which you can then put in a sulfur geyser to make lye.
>Lye would be used as a damaging water that doesn’t hurt you as much as lava, but also allows you to boat on it, as well as not destroying items you throw in it, making it perfect for trap moats and defense. Brittle ice would break faster in it, packed ice would melt, ice would melt faster, and blue ice would convert it back to water. But it’d also clean copper and any other “oxidizables” they may or may not add later on

**Example 2: Phantom Reworks**
>Idea for how phantoms should work:
>Preface
>The phantom should spawn at night ALWAYS, but it's behavior depends on if a player nearby (within 8 chunks maybe?) has slept
>With Sleeping
>When a player has slept, phantoms should not attack the player unless attacked, and during the day they should become become more and more translucent until they despawn (maybe like 8 seconds of disappearing) entirely without dropping anything. They can be killed, but it should be hard to reach or hit them, with them very slightly trying to avoid players, but not that much, and they try to remain at maybe around y=200. There should be a limit of around 3 per 20 chunks, with the same despawning applying if the limit exceeds.
>Without Sleeping
>When a player has not slept for a minimum of 3 days, the phantom gets hostile, gaining hostility as the nights go on. They should die during the day always. With 3 days, it should try to remain at around y=175, and should swoop down every maybe 30 seconds? Dealing 2 damage. Next hostility could be 6 days, where they try to remain at around 150, and swoop every ~12 seconds, dealing 4 damage. Next and final hostility should be ~12 days, with them remaining at around 100, swooping every 4 seconds, and dealing 12 damage.
>These values should be changed to better suit balancing, I just made them up because I can't play Minecraft or create this as a mod for the next few days. Give suggestions please!! Also this was not generated with an llm don't accuse me of that

### `pitch`

**Definition: A spec that also engages with at least one consequence: a downside or balance concern, why an existing feature doesn’t already solve the problem, or how it interacts with existing mechanics.**

**Example 1: Ice Caves Rework**
>The new Ice Caves are super cool (no pun intended), but with so many hostile features to survival players, it’s hard to understand the trade off for this biome.
>The Frostbite zombies can freeze you and have ranged Ice ball attacks. Lighting up the caves causes ice to melt which makes ice spikes fall on you. And now with the brittle ice that upon stepping on, one can fall a significant distance. They also may add the Iceologer which would make the biome even more dangerous.
>So what’s the point of even going here besides collecting ice-type resources? Sure, ores are easier to see, but literally anywhere else would be less hostile.
>I’m going to recommend the Ice Caves get a significant buff in the form of ore spawn rates. Specifically, I think a proper tradeoff could be increased Diamond spawn rates. Similarly to how Gold spawns more in Mesas, Diamonds could spawn more (and higher up) in Ice Caves.
>With great risk should come great reward, and diamonds already are hard to find with no renewable way to obtain them— so having them spawn more in this biome would give survival players a locale to specifically look for them. It also obviously gives players more of an incentive to engage with the new biome.
>This part is superfluous: but also diamonds match the “color scheme” for the ice caves. And yeah I know that diamonds realistically should spawn in “hotter” areas but like when has Minecraft ever cared about geological realism haha.


**Example 2: Make all equipment upgradeable to higher tiers**
>Mojang has said before that they consider impermanence to be important as part of the game design. They clearly want the player to not keep armor around and to be ok with letting it break, then build new sets and get different enchantments. That would be why mending is so hard to come by, and also why the enchanting table largely has random rolls, plus why you practically have to build an XP farm to repair things with the anvil.
>But in practice, we all know that isn't how things go. The player quickly discards iron armor for diamond, then keeps the diamond around for netherite upgrades since netherite is rare and expensive. After getting netherite, the player is heavily incentivized to grind for mending despite its rarity, because of the aforementioned difficulty involved in collecting more netherite for repairs. Because of the difficulty involved in netherite upgrades, as well as the requirement of having certain tiers of tools to collect certain resources, this game design decision actually incentivizes keeping an end-game tool around forever and also encourages hoarding enchantments for this end game gear. It also leads to the thoughtless discarding of old equipment as well as largely perceiving many loot chest tools as being total trash. After all, why would you wanna pick up a gold pickaxe or a stone axe unless you were just starting?
>So, how do we resolve this problem? Simple. The game design needs to change in a way that allows easier upgradeability. If it is easier and cheaper to get ahold of better tools, especially if it utilizes old ones, the player would have an easier time with the idea of letting better tools break. Importantly, this design change would allow players to keep a set of armor, weapons and tools, but also ensure that it is not as big of a deal to lose them.
>The biggest change I would make on this front is the ability to upgrade tools from their current tiers into higher ones. Although the player could still, for instance, craft a diamond pickaxe outright, they could instead play more resourcefully and use 1 diamond to upgrade an iron pickaxe to diamond, carrying over enchantments and repairing it. This would ensure both that the pickaxe doesn't get discarded to a random chest or smelted for 1 iron nugget, while also making sure that it isn't a tragedy to lose a diamond pickaxe. After all, iron is significantly more common and you are much more likely to have a double chest full of it than diamonds. Being 1 diamond away instead of 3 would be a huge incentive to not worry about preserving it.
>On top of that, I am in favor of nixing the XP cost for repairing your equipment. While in Mojang's original game design this served as a way to dissuade players from keeping equipment around, the upgrade system serves as a far larger incentive. As a result, since the player is no longer as concerned with permanence, this artificial barrier can be safely removed. XP already has enough use for enchanting.
>To resolve the netherite problem, I think an overhaul in how the player acquires it is in order. Ancient debris mining is actually insane. Strip mining is largely the only way to get ahold of large quantities, and yet Jeb said lava pockets were added to dissuade it. Like, what? Is the player supposed to spend 100 hours wandering aimlessly in the nether to find debris and scraps in bastions, and then have to keep doing that further and further out in order to build new sets? I honestly have no idea what they were thinking with this game design choice, and so I am nixing lava pockets and also overhauling debris. Now, debris drops scrap when mined, and it is affected by fortune. If the player wants to collect debris, they have to use silk touch. This has the additional interesting choice of collecting debris in order to save it for when the player gets a fortune roll from the enchanting table or a book.
>The game should also give the player more avenues for collecting debris or netherite. They could be an extremely rare trade with piglins for example, and their generation could be changed to be in line with overworld mining, ie, it generates more often with the flow of nether generation and less in a way that requires strip mining. If it was changed in the overworld because strip mining isn't very fun, it should also change in the nether.
>Additionally, less scrap is now required to make netherite, and if you have golden armor, you can skip the gold-fusing part of the crafting recipe. May as well make gold more useful, seeing as it is almost entirely worthless currently beyond preventing piglin aggro.
>Alongside these changes, I think it is only fair to be able to get more materials out of armor and tools when smelting them. After all, if Mojang wants these things to be impermanent, you should be able to get more out of discarded sets. Otherwise, the game design feeds back into rewarding keeping a set forever. Durability determines how many ingots or nuggets you get out of smelted tools, weapons, and armor now, and you can also use books to pull good enchantments off of equipment to use for later. This has the additional perk of encouraging players to pick up equipment that otherwise is usually considered useless from loot chests. That golden pickaxe is now at least a couple gold ingots and a good enchanting book away!
>I think some other conceptual changes that might help would be more conditional/environmental hazards that require the player to have multiple armor sets for different purposes. Make sure to have leather armor when exploring around powdered snow, to prevent cold damage. Avoid outright metal armor in the nether, because it is hot and metal is conductive. Copper armor could attract lightning or power redstone contraptions. Maybe they could even add a progression fork that allows for either netherite or something else, perhaps from the Sift. This would allow for more customization as well as more choices in how you tackle the sandbox, and would also encourage crafting armo sets the player normally wouldn't.
>I would also consider adding netherite upgrades for more items (ie, the trident, the mace, the bow, golden apples, etc), which would give the player more incentives to get ahold of a lot.
>I think it also may be worth weakening the shield and adding shield tiers instead that increase its durability and decrease the block cooldown.

### The hardest boundary

**Which two labels: `spec` and `pitch`**

**The decision rule I used every time:**
A post is pitch only if it is already a spec and it weighs something other than the idea itself: a downside or side effect of the change, an existing feature presented as a possible answer and explained as falling short, or an interaction with current mechanics. Otherwise it’s spec.



---

## The Dataset

<!-- Where you collected from, how you labelled, your counts, and three hard
     cases. -->

**Where the posts came from: r/minecraftsuggestions**

**How I labelled them: I first cold labelled 20 by hand, then had Claude label the rest.** <!-- Cold first? Pre-labelled with AI and corrected?
Say so plainly — the disclosure is required, not penalised. -->

**Counts per label:**

| Label | Count | Share |
|---|---|---|
| `wish` | 85 | 42.5% |
| `spec` | 68 | 34.0% |
| `pitch` | 47 | 23.5% |
| **Total** | 200 | 100% |

**Three hard cases**

<!-- Any post that made you pause: what it was, which two labels it could have
     been, and what you chose. These are worth more than the easy 190. -->

**1.**
> *The post:* "Right-clicking a furnace with flint and steel keeps it lit permanently". It's a short cosmetic tweak: the furnace stays lit until broken, and it applies to smokers and blast furnaces too. The author adds, "No, it wouldn't infinitely smelt items, it would purely be cosmetic, you still have to put fuel in like normal."
>
> *Could have been:* `spec` or `pitch`
>
> *I chose, because:* `pitch`. The post is short, but the behavior is fully pinned down, so it is at least a `spec`. The "no infinite smelting" line heads off an exploit, so it weighs a side effect of the change. Under my rule, that makes it a `pitch`, even though it reads like a one-liner.

**2.**
> *The post:* "Increase the cushion health". Cushions take many steps to set up and break when you misclick, so "the cushion should need at least 3 hits."
>
> *Could have been:* `wish` or `spec`
>
> *I chose, because:* `wish`. It gives a concrete number, so two readers would picture almost the same thing. But the whole change is one clause ("needs 3 hits"), and my `wish` definition covers a whole change that is one clause. The reasoning is only a motive, so it doesn't push the post any higher.

**3.**
> *The post:* "Ice Mansion - Illager Mansion in the Ice Caves". It describes a rare Woodland-Mansion-like structure in Ice Caves with reskinned illagers. Iceologers replace Evokers, "having a new set of ice-themed moves that makes them just as dangerous as Evokers."
>
> *Could have been:* `wish` or `spec`
>
> *I chose, because:* `spec`. Most of the post is defined by reference to an existing structure (same shape, same loot, same illagers apart from clothing), so readers would picture the same thing. The Iceologer's moves are never described, which pulls it toward `wish`. Still, that is one missing detail, not the core behavior.

---

## The Training Run

<!-- Your starting model, your settings, and anything you changed and why. -->

**Base model:** `distilbert-base-uncased`

**Settings:** <!-- epochs, learning rate, batch size, seed -->
3 epochs, learning rate 2e-5, batch size 16, max length 128 tokens, seed 42. Trained on CPU (torch 2.14.1+cpu).

**Anything I changed from the defaults, and why:**
Nothing. I kept every default so the first run is a clean baseline to compare later changes against.

One default is worth flagging: `MAX_LENGTH = 128`. My posts are long, and 128 of the 200 (64%) run past 128 tokens and get truncated. That includes 58 of 68 `spec` posts and 38 of 47 `pitch` posts, but only 32 of 85 `wish` posts. The part that makes a post a `pitch` (a downside, a balance concern, or an interaction with existing mechanics) usually comes after the mechanics are described. So it is often in the part the model never sees, which fits `pitch` scoring 0 F1 on this run.

**Split sizes:** <!-- train / val / test, and per-label counts in the test
split. If a label had fewer than about 8 in test, say so — it explains a lot
of next unit's variance. -->
Stratified 70/15/15 split with seed 42: **train 139 · val 31 · test 30**.

| Label | Train | Val | Test |
|---|---|---|---|
| `wish` | 59 | 13 | 13 |
| `spec` | 47 | 11 | 10 |
| `pitch` | 33 | 7 | 7 |

`pitch` has only **7** examples in the test split (under 8), so its F1 will swing a lot between seeds. On this run the model predicted `pitch` zero times. All 7 `pitch` posts and 6 of 10 `spec` posts were called `wish`, which gives 0.567 accuracy and 0.413 macro F1 (`results.json`).



---

## How I Used AI

<!-- Two specific moments — what you asked, what came back, what you changed.

     ⚠️ Plus disclosure of any pre-labelling. If you had a model pre-label a
     batch and then read and corrected every one, say that. It's an allowed
     workflow and disclosing it costs you nothing. Not disclosing it is the
     problem. -->

**Moment 1**

- *What I asked for: Evaluation of my 3 proposed labels, problem, wish, spec*
- *What came back: A preliminary evaluation of the subreddit and noting that problem type posts were actually not that common.*
- *What I changed: Removal of the problem label and addition of the pitch label.*

**Moment 2**

- *What I asked for: Help scraping posts off of the subreddit and labelling.*
- *What came back: Mostly correct labels, but some one off posts that needed correcting*
- *What I changed: Corrected post labels, noted in `labels.csv`*

**Pre-labelling disclosure: I hand-labelled 20 posts, then asked Claude to scrape and label the rest, after which I reviewed them.**

<!-- ═══════════════════════ UNIT 6 — THE TEST ═══════════════════════

     Don't fill these in during unit 5.
     ═══════════════════════════════════════════════════════════════════ -->

---

## Baseline vs. Trained

<!-- Both models on the same posts. `python baseline.py --trained results.json`
     prints this table for you. -->

| Measure | Baseline | Trained | Difference |
|---|---|---|---|
| Overall accuracy |  |  |  |
| Macro F1 |  |  |  |
| F1 — `label_one` |  |  |  |
| F1 — `label_two` |  |  |  |

**What I predicted before I looked:**
<!-- Milestone 1 asks you to write this BEFORE seeing the trained numbers. A
     prediction made afterwards isn't one. -->

**What the gap actually means:**
<!-- If the baseline matched your trained model, your fine-tuning added
     nothing — and that is a real finding, not a failure. Say it plainly. -->



---

## Run Log — Before

<!-- Five criteria across three seeds. The notebook's section 6 prints the
     spread table; the Target and Verdict columns are yours. -->

| Criterion | Target | Seed 42 | Seed 7 | Seed 2024 | Verdict |
|---|---|---|---|---|---|
| 1.  |  |  |  |  |  |
| 2.  |  |  |  |  |  |
| 3.  |  |  |  |  |  |
| 4.  |  |  |  |  |  |
| 5.  |  |  |  |  |  |

### Confusion matrix

<!-- ⚠️ TYPED AS A MARKDOWN TABLE. The notebook prints one ready to paste.
     An image of a matrix earns nothing. -->

| true \ predicted |  |  |  |
|---|---|---|---|
| **** |  |  |  |
| **** |  |  |  |
| **** |  |  |  |

**My biggest off-diagonal number, and what it means:**
<!-- Not "the model made mistakes" — WHICH boundary it didn't learn, and which
     direction. "7 real analysis posts were called hot_take and only 3 went the
     other way" is a direction, not just an error rate. -->



---

## Verdicts and Diagnoses

<!-- MET or MISSED against LAST UNIT's target. The target has to hold across
     all three seeds, not turn up sometimes. -->

| # | Criterion | Target | Verdict | How I decided |
|---|---|---|---|---|
| 1 |  |  |  |  |
| 2 |  |  |  |  |
| 3 |  |  |  |  |
| 4 |  |  |  |  |
| 5 |  |  |  |  |

**Diagnoses**

<!-- For each miss: the cause, and how you know. The four common causes are:
     too few examples for a label, a boundary you applied inconsistently, a
     genuinely hard label pair, and a task the model can't reach from this
     much data.

     ⚠️ Use your agreement report as evidence. It is the only instrument you
     have that can tell a LABELLING problem from a MODEL problem, and this
     section is graded on whether you used it that way. -->



---

## Agreement Report

<!-- Your rate against the staff set, and every disagreement adjudicated.

     Remember you labelled these 30 under the STAFF taxonomy in
     data/staff_taxonomy.md, not your own — so every argument below is made
     from those definitions and those decision rules. -->

**Agreement rate:** ___ / 30 = ___%

<!-- Nobody grades this number. A 60% who argues every disagreement from the
     stated rules beats a 95% who wrote "staff was right" nine times. Several
     of the 30 were chosen because they're genuinely ambiguous — you should be
     winning some of these. -->

**Disagreements**

<!-- Three lines each: the post, both labels, and who you think is right and
     why — grounded in the staff definitions you were both applying.

     Then sort each into one of three piles:
       (a) the rule covered it and I applied it loosely → a consistency problem
       (b) the rule genuinely doesn't say               → a gap in the definitions
       (c) the rule is ambiguous here and my reading is defensible → argue it.
           This is a legitimate win.

     Pile (a) is the one that matters most for your diagnosis: if you applied a
     written rule two different ways on 30 posts, that is direct evidence about
     what you did across your own 200. -->

**1.**
> *The post:*
>
> *Staff said / I said:*
>
> *My call, and why:*
>
> *Which pile:*

**2.**
> *The post:*
>
> *Staff said / I said:*
>
> *My call, and why:*
>
> *Which pile:*

**What the pattern in my disagreements tells me:**



---

## The Improvement

**What I changed:**

**Which diagnosis pointed at it:**

### Run Log — After

| Criterion | Target | Seed 42 | Seed 7 | Seed 2024 | Verdict |
|---|---|---|---|---|---|
| 1.  |  |  |  |  |  |
| 2.  |  |  |  |  |  |
| 3.  |  |  |  |  |  |
| 4.  |  |  |  |  |  |
| 5.  |  |  |  |  |  |

**Did it help, and how do I know:**

<!-- If it didn't, say so. Relabelling that didn't help is a genuinely
     interesting result and earns full credit. -->



---

## What's Still Broken

<!-- For each criterion still missed: what you'd do, and why you stopped. -->



**The gap between what I meant my labels to capture and what the model
learned:**
<!-- Two sentences. Your confusion matrix is the evidence. -->



<!-- ═════════════════════════════════════════════════════════════════════

     SUBMISSION CHECKLIST — unit 5

       [ ] criteria.md has five numbered criteria, each naming a NUMBER
       [ ] Each has a reason underneath tied to your data or taxonomy
       [ ] labels.csv: at least 150 rows, text/label/note, ONE file not split
       [ ] No label above 70%
       [ ] All five unit 5 sections have real content
       [ ] Label Taxonomy includes the decision rule for your hardest boundary
       [ ] The Dataset includes three hard cases
       [ ] results.json and test_split.csv committed (the notebook does this)
       [ ] At least four new commits
       [ ] Repository URL submitted — WRITE IT DOWN

     SUBMISSION CHECKLIST — unit 6

       [ ] Baseline vs. Trained table, with your prediction written beforehand
       [ ] Run Log — Before, five criteria across three seeds
       [ ] Confusion matrix TYPED AS A MARKDOWN TABLE
       [ ] A verdict on every criterion
       [ ] A diagnosis for every miss, using the agreement report as evidence
       [ ] Agreement Report with every disagreement adjudicated
       [ ] One improvement, with Run Log — After
       [ ] What's Still Broken
       [ ] results_three_seeds_before.json, results_three_seeds_after.json,
           baseline_results.json and
           agreement_results.json committed
       [ ] At least four new commits
       [ ] The SAME repository URL as last unit

     Do not delete and recreate this repository.
     ═════════════════════════════════════════════════════════════════════ -->

---

📖 **How to run this project: [RUNNING.md](RUNNING.md)**
