# Overpower and Possession

## Overpower

Overpower (OP) is an indicator that was introduced in Chunithm STAR PLUS, and it acts as a sort of "global completion marker" for the game. It is calculated from the best score on each chart compared to the theoretical maximum.

The Overpower indicator can be toggled in **settings**.

![Overpower indicator](images/overpower.png)

The way that overpower is determined is not relevant for most players, but it does have some involvement with the possession system (see below). Generally speaking, you need to try and get as many charts as close to their theoretical maximum value (All Justice Critical) as possible to reach maximum overpower.

Overpower scales primarily based on the chart constant, but most OP gain is held **beyond the SSS score threshold**. About 5-6% of OP on a given chart will remain in the 2500 points beyond SSS, which itself only accounts for 0.3% of the total score. Additionally, combo frames contribute an extremely significant amount of overpower, detailed below:

- Full Combo = +0.5 OP
- All Justice = +1.0 OP
- All Justice Critical = +1.25 OP

![Chart of score vs. OP gain](images/score-op.png)

A table detailing benchmark scores required to reach Possession thresholds across a sampling of difficulties is shown below.

![OP score table](images/op-table.png)

### Overpower Calculation/Display (~LUMINOUS)

The Overpower tracking system was overhauled in accordance with the Ultima system changes made to this version. Pre-LUMINOUS+, overpower was calculated for every **individual chart**, and the player would have been able to see their Overpower metrics for whatever folder and difficulty was active at the time. For instance, a score on an Expert chart would contribute to Expert OP% but would not contribute to possession (which only considered Master OP and Ultima OP).

Note how the Overpower value displayed is different between Expert difficulty and Master difficulty.

![Lumi Exp OP](images/OP-lumi-1.png)
![Lumi Mas OP](images/OP-lumi-2.png)

### Overpower Calculation/Display (LUMINOUS+~)

Overpower metrics are now calculated for the **song**, regardless of the difficulty. For each song, the score that would result in the **highest OP** value contributes to Total OP. This is typically the score on the highest played difficulty, but in some instances a very high score on a lower difficulty chart may provide more OP than a poor score on a higher difficulty chart.

The Total OP is now calculated from the theoretical value (AJC) on the highest available difficulty across all songs in the folder.

![Lumi+ OP Change Description](images/OP-lumi-plus-desc.png)

Folders will likewise display the **Total OP** gained on the folder instead of being bound by the difficulty. The two photos below show the same Overpower number and OP%, but different clear lamps.

![Lumi+ Exp OP](images/OP-lumi-plus-1.png)
![Lumi+ Mas OP](images/OP-lumi-plus-2.png)

Additionally, the Random tab in song select will now display **Total OP and OP%**. The rank/combo lamps displayed in this view will change with the selected difficulty.

![Lumi+ Mas Total OP](images/OP-lumi-plus-all.png)

Details about overpower breakdown (including the calculation formula) can be found on [wikiwiki](https://wikiwiki.jp/chunithmwiki/%E3%83%AC%E3%83%BC%E3%83%86%E3%82%A3%E3%83%B3%E3%82%B0%E3%83%BBOVER%20POWER).

## Possession

Rating possession is an indicator that was introduced in Chunithm AMAZON PLUS. Achieving a rating possession will change the portion of the player card that includes the player tag, level, rating, and class badge/banner to have a silver, gold, platinum, or rainbow background depending on specific requirements. These requirements include achieving a **minimum rank** on **all Master charts** (and Ultima charts in New and above) **in the entire game**.

| Possession Type | Player Card                                                                     |
| :-------------- | :------------------------------------------------------------------------------ |
| Silver          | ![Silver possession indicator](images/pos-silver.png){: style="width: 300px"}   |
| Gold            | ![Gold possession indicator](images/pos-gold.png){: style="width: 300px"}       |
| Platinum        | ![Platinum possession indicator](images/pos-plat.png){: style="width: 300px"}   |
| Rainbow         | ![Rainbow possession indicator](images/pos-rainbow.png){: style="width: 300px"} |

The conditions for achieving rating possession are as follows:

| AMAZON+~CRYSTAL |                |              |                 |
| --------------- | :------------: | :----------: | :-------------: |
| **Colour**      |   **Rating**   |   **Rank**   | **OP required** |
| Silver          | 15.25 or above |  S or above  |       N/A       |
| Gold            | 15.50 or above | SS or above  |       N/A       |
| **Rainbow**     | 15.75 or above | SS or above  |      99.5%      |

| CRYSTAL+~PARADISE LOST |                |             |                 |
| ---------------------- | :------------: | :---------: | :-------------: |
| **Colour**             |   **Rating**   |   **Rank**  | **OP required** |
| Silver                 | 15.25 or above |  S or above |       N/A       |
| Gold                   | 15.50 or above | SS or above |       N/A       |
| Platinum               | 15.50 or above | SS or above |      98.5%      |
| **Rainbow**            | 15.75 or above | SS or above |      99.5%      |

| NEW~NEW+    |                 |             |                 |
| ----------- | :-------------: | :---------: | :-------------: |
| **Colour**  |   **Rating**    |   **Rank**  | **OP required** |
| Silver      | 16.25 or above  |  S or above |       N/A       |
| Gold        | 16.50 or above  | SS or above |       N/A       |
| Platinum    | 16.50 or above  | SS or above |      98.5%      |
| **Rainbow** | 16.75 or above  | SS or above |      99.5%      |

| SUN~SUN+    |                    |              |                 |
| ----------- | :----------------: | :----------: | :-------------: |
| **Colour**  |   **Rating**       |   **Rank**   | **OP required** |
| Silver      | 16.25 or above     |   S or above |       N/A       |
| Gold        | 16.50 or above     |  S+ or above |      97.5%      |
| Platinum    | 16.**75** or above | SS or above  |    **99.3**%    |
| **Rainbow** | 16.75 or above     | SS+ or above |    99.**6**%    |

| LUMINOUS    |                    |              |                 |
| ----------- | :----------------: | :-------- -: | :-------------: |
| **Colour**  |   **Rating**       |   **Rank**   | **OP required** |
| Silver      | 16.25 or above     |   S or above |       N/A       |
| Gold        | 16.50 or above     |  S+ or above |      97.5%      |
| Platinum    | 16.75 or above     | SS or above  |   **98.85**%    |
| **Rainbow** | **17.00** or above | SS+ or above |   99.6**2**%    |

| LUMINOUS+   |                |                  |                 |
| ----------- | :------------: | :--------------: | :-------------: |
| **Colour**  |   **Rating**   |     **Rank**     | **OP required** |
| Silver      | 16.25 or above |     S or above   |       N/A       |
| Gold        | 16.50 or above |    S+ or above   |      97.5%      |
| Platinum    | 16.75 or above |   SS or above    |   **99.00**%    |
| **Rainbow** | 17.00 or above | **SSS** or above |   99\.**50**%   |

| VERSE~X-VERSE |                    |              |                 |
| ------------- | :----------------: | :----------: | :-------------: |
| **Colour**    |     **Rating**     |   **Rank**   | **OP required** |
| Silver        | **16.00** or above |   S or above |       N/A       |
| Gold          | **16.00** or above |  S+ or above |      97.5%      |
| Platinum      | **16.00** or above | SS or above  |     99.00%      |
| **Rainbow**   | **16.00** or above | SSS or above |     99.50%      |

_Credit to beerpsi for finding accurate possession thresholds and values_

If you see anyone with a possession plate, you can tell that they've sunk a lot of time into the game. I encourage players who are passionate about Chunithm to go for at least Silver possession—the experience of playing through all of the different patterns in the game is helpful for solidifying fundamentals.
Ddrlevelasian’s [CHUNITHM Possession Guide](https://docs.google.com/document/d/1wCRvaoXezTfqFLwY9bssxgWifvOHXJC6jt_mi0QrutQ/edit?usp=sharing) is a fantastic read if you are at all curious about what the process of possession is like and how it can benefit you as a player.
