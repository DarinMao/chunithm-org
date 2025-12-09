# Rating and Meta-Progression

After playing your first few credits of the game, you might find yourself asking: "That was fun, but how do I get better?"

As you've probably noticed, your player card displays a rating, which is a numerical approximation of your skill. In general, setting higher scores on higher difficulty maps will increase the rating value. However, the system is quite deep and requires some explanation to fully understand.

## Rank/Colour

The colour of the rating is dependent on which rating bracket it falls into.

| **Rating**     | **Colour**  |
| :------------- | :---------- |
| 0.00 to 3.99   | Green       |
| 4.00 to 6.99   | Orange      |
| 7.00 to 9.99   | Red         |
| 10.00 to 11.99 | Purple      |
| 12.00 to 13.24 | Bronze      |
| 13.25 to 14.49 | Silver      |
| 14.50 to 15.24 | Gold        |
| 15.25 to 15.99 | Platinum    |
| 16.00+         | **Rainbow** |

??? "Legacy Rating (~**PARADISE LOST**)"

    | ~PARADISE LOST |             |
    | :------------- | :---------- |
    | **Rating**     | **Colour**  |
    | 0.00 to 3.99   | Green       |
    | 4.00 to 6.99   | Orange      |
    | 7.00 to 9.99   | Red         |
    | 10.00 to 11.99 | Purple      |
    | 12.00 to 12.99 | Bronze      |
    | 13.00 to 13.99 | Silver      |
    | 14.00 to 14.49 | Gold        |
    | 14.50 to 14.99 | Platinum    |
    | 15.00+         | **Rainbow** |

**VERSE**: rating intervals of 0.25 past **Platinum** are recognized with stars.

| Rating | Rank                                                                                           |
| :----- | :--------------------------------------------------------------------------------------------- |
| 16.00  | Rainbow (★)<br>![Rainbow 1 rank up](images/rainbow-1.png){: style="width: 200px"}              |
| 16.25  | Rainbow (★★)<br>![Rainbow 2 rank up](images/rainbow-2.png){: style="width: 200px"}             |
| 16.50  | Rainbow (★★★)<br>![Rainbow 3 rank up](images/rainbow-3.png){: style="width: 200px"}            |
| 16.75  | Rainbow (★★★★)<br>![Rainbow 4 rank up](images/rainbow-4.png){: style="width: 200px"}           |
| 17.00  | Rainbow (極, "Kiwami")<br>![Rainbow Kiwami rank up](images/kiwami.png){: style="width: 200px"} |

## Rating Formula (VERSE~)

**VERSE**: the recents folder has been **removed**. Instead, rating is composed of a "new songs" folder alongside the existing "best rated scores" folder, similar to maimaiDX.

Rating is now measured across **50 charts** in total. You can no longer have your rating drop at any point during the active version, although players can expect their rating to drop upon the next version of the game (Chunithm VERSE PLUS).

The player rating formula is split up into two components:

| Top 30 all-time scores | \+  | 20 high scores from current version |
| :--------------------: | :-: | :---------------------------------: |
|   aka "Best 30/B30"    |     |          aka "New 20/N20"           |

All individual charts must be **unique** across all rating charts. In other words, a high score on a chart that would contribute to your B50 would only count once.

The amount of **rating** gained for charts is dependent on two variables: the **chart constant** and the **score** achieved on the chart.

The table below illustrated how much rating is gained at each rank threshold:

| Rank             | Score     | Rating value              |
| ---------------- | --------- | ------------------------- |
| SSS+<sup>1</sup> | 1,009,000 | Chart constant \+2.15     |
| SSS              | 1,007,500 | Chart constant \+2.0      |
| SS+              | 1,005,000 | Chart constant \+1.5      |
| SS               | 1,000,000 | Chart constant \+ 1.0     |
| S                | 975,000   | Chart constant (+ 0\)     |
| AA               | 925,000   | Chart constant \- 3.0     |
| A                | 900,000   | Chart constant \- 5.0     |
| BBB              | 800,000   | (Chart constant \- 5.0)/2 |
| C                | 500,000   | 0                         |

_<sup>1</sup>Note: The SSS+ bonus interval, similar to other \+ intervals, is only in Chunithm NEW and later ([Score Evaluation](../basic/evaluation.md)); the cap for PARADISE LOST is \+2.0._

Scores that lie in between these thresholds are **interpolated**, see the "Gaining Rating" section below.

??? "Legacy Rating Formula (~LUMINOUS+)"

    The **player rating formula** is split up into two components:

    | Top 30 all-time scores | \+  | Recent 10 high scores |
    | :--------------------: | :-: | :-------------------: |
    |   aka "Best 30/B30"    |     |     aka "Recents"     |

    An example is shown below (source: [Chunithm Rating Calculator](https://docs.google.com/spreadsheets/d/1TT3-89PqcTvyL_nMbnGxL2q5bg5pLtHiKg_qStSJ88M/edit#gid=824923779)):
    ![Rating calculator screenshot](images/rating-calc.png)

    Charts in the **Top 30** must be unique (only one entry per chart). You may have two difficulties of the same song in the Top 30, but not the same difficulty. Charts in **Recents** are not held to any such restrictions and as such you may fill the Recents section with multiple plays of the same chart. Recents are taken from the last **30** charts played and will be displaced either once a score with a higher rating is achieved or 30 new charts have replaced the pool.

    !!! mitsuyoshi "Mitsuyoshi Tip!"
        <strong id="mitsuyoshi-7">SSS "Rating Guard"</strong>

        Another factor in the recents rule is that scores of rank SSS or above (of any difficulty) will **not** displace the recent 10, instead pushing out the oldest chart amongst the remaining 20 in the recents pool. This is why you usually do not drop rating on SSS scores as the developers anticipated it wouldn't be very player friendly. As soon as a non-SSS score is achieved, the normal rules apply and the oldest chart in recent 10 is displaced. Exceptions are possible.

## Gaining Rating

The maximum possible rating you can get from a chart is the **chart constant +2.15**, so any additional score after 1,009,000 no longer contributes to your rating. Let's examine how much rating you gain at each interval, shall we?

| Rank | Score                  | Rate of increase               |
| ---- | ---------------------- | ------------------------------ |
| SSS+ | 1,009,000 ~            | 0                              |
| SSS  | 1,007,500 to 1,008,999 | +0.01 for every 100 points     |
| SS+  | 1,005,000 to 1,007,499 | +0.1 for every **500** points  |
| SS   | 1,000,000 to 1,004,999 | +0.1 for every **1000** points |
| S+   | 990,000 to 999,999     | +0.1 for every 2500 points     |
| S.   | 975,000 to 989,999     | +0.1 for every 2500 points     |

![Chart of rating gain vs. score](images/score-rating-gain.png)

We can see from this table that rating increases linearly up to SS rank, where the rate at which rating is gained jumps by 2.5x. If we look at the interval between SS+ and SSS, the rate jumps yet again to 5x! This shows that the **highest value** interval to target for gaining rating from charts is **SS+ to SSS**. As such, I highly recommend **aiming for SSS rank** when trying to improve at the game. Not only does this contribute the largest amount of rating, but by being more deliberate with your play and fully understanding patterns, you will improve at a faster pace and avoid building bad habits.

## Skill Floor, Skill Ceiling/Pull-Run-Push

_aka how to structure your play sessions_

I suggest taking a balanced approach to develop a more well-rounded skillset. In my opinion, you should primarily focus on **playing charts that you can SS+/SSS** (as stated above, since that's where most rating gain occurs). A quick benchmark to determine what level that is to take your peak rating, subtract 2, then round it to the nearest 0.5; that will roughly determine what level your "run" level is at.

_E.g. Player rating of 14.9 > 14.9 - 2 = 12.9 > round up 12.9 to 13; primarily play around level 13_

You should also take some time occasionally to play charts that are a level or two **underneath** your standard difficulty range and aim for SSS+ or All Justice to increase your **skill floor**, and similarly sometimes play charts that are a level **higher** than your standard difficulty to increase your **skill ceiling**. This balance of playing charts across a spectrum of difficulty with different goals is also referred to as **pull-run-push**.

Improving your skill floor (aka "playing lowers") is important in order to develop more accurate timing and solidify fundamental patterns. Nearly every single chart in the game has something to teach you, even if you aren't feeling challenged for the majority of the chart. The more you do this, the easier it becomes to eventually get All Justice on higher difficulties.

Improving your skill ceiling (aka "skill pushing", "playing uppers") is also good in moderation to expose you to new patterns that you haven't seen and give you a taste of what lies ahead in the game. Most players would agree that the really fun charts are confined largely to higher difficulties, as that's where chart creators can throw in more demanding patterns, homages to other charts, and chart-specific tech that will take you by surprise on sightread.

This theory is expanded upon in the [_Mentality for Improvement in Rhythm Games_](https://docs.google.com/document/d/1gwuauPmfOTm99oOQlbZLBDRdIHUHi0Mnz3UW3hImmNc/edit) article written by 8por?:

"_In order to prevent burnout and maintain interest, it's best to keep a balance of pushing the skill floor and skill ceiling. An proven effective pattern is pull-run-push cycle, which includes warming up/pulling the floor → solidifying skill by playing at the optimal difficuly level → pushing the ceiling. It's recommended to plan your sessions around this pattern._" \- 8por?

As an example of what this looks like in a play session, I'd suggest playing 1-2 sets of lower difficulty charts to warm up followed by a mix of standard difficulty charts with some upper difficulty charts thrown in. For instance, for a 15.1 rated player (gold rating), consider the following:

- Set 1: 12 > 12 > 12+
- Set 2: 12 > 12+ > 12+
- Set 3: 13 > 13+ > 13
- Set 4: 13+ > 13 > 14
- Set 5: 13 > 13+ > 14

This article with the same name ([_Skill Floor, Skill Ceiling_](https://iidx.org/theory/skill_ceiling_floor)) written by Horie is a fantastic reference that expands upon this idea in more detail despite being written for beatmania iidx.

!!! mitsuyoshi "Mitsuyoshi Tip!"
    <strong id="mitsuyoshi-8">A comprehensive-ish set of goals to improve at all stages of progression</strong>

    "Help! There's too much information to follow. Can you just give me a discrete set of goals to work on at \[insert rating here\]?"

    In fact, I can! I've put together a mix of progression goals and task chart with fellow Chunithm player underjoy, and you can find it in the [Kamaitachi Chunithm Questline Tracker](https://chunithm.org/quests). It was designed to help players develop mastery and become well-rounded at all areas of the game, and it should provide an ample challenge to those seeking one.
