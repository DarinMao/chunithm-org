# Timing Windows

The timing window is different for the different note types, each corresponding to a judgement type. All values are in milliseconds (ms).

_Tables adapted from the [donmai blog](https://listed.to/@donmai), link to his article containing [Chunithm timing windows](https://listed.to/@donmai/41511/gekichumai-timing-windows-and-offsets) (in addition to Maimai and Ongeki) here._

## Tap Timing Windows

| Note Type  | Justice Critical | Justice       | Attack        | Miss    |
| ---------- | ---------------- | ------------- | ------------- | ------- |
| Tap        | < 33.33          | 33.33 < 66.67 | 66.67 < 83.33 | > 83.33 |
| Extap      | < 83.33          | N/A           | N/A           | > 83.33 |
| Tap Easy   | < 33.33          | 33.33 < 66.67 | 66.67 < 100   | > 100   |
| Extap Easy | < 100            | N/A           | N/A           | > 100   |

Tap/Extap Easy are expanded timing windows for BASIC and ADVANCED difficulty charts. EXPERT and above difficulties follow the first two lines.

## Hold Timing Windows

| Note Type       | Justice Critical | Justice    | Attack      | Miss   |
| :-------------- | :--------------- | :--------- | :---------- | :----- |
| Hold/Slide Tick | -50 < 0          | -100 < -50 | -150 < -100 | < -150 |

The initial input on holds and slides has the same timing window as a tap note. The game measures holds at ticks or "checkpoints" within the hold or slide, and the difference between last input and the tick determines the judgement type. For instance, you can let go and fall back on a hold within the timing window and maintain justice judgements.

## Flick Timing Windows

| Note Type   | Justice Critical | Justice        | Attack   | Miss    |
| :---------- | :--------------- | :------------- | :------- | :------ |
| Flick Tap   | < 33.33          | 33.33 < 83.33  | N/A      | > 83.33 |
| Flick Slide | < 83.33          | 83.33 < 166.67 | > 166.67 | N/A     |

Flicks are separated into two phases: the initial tap and the following slide motion. Failure to do the slide phase of the flick after hitting the tap phase will result in a slow attack. Note that the actual judgement is given to the flick as a whole, and not these two separate parts.

## Air Timing Windows

| Note Type           | Fast Attack       | Fast Justice   | Justice Critical | Late Justice | Late Attack     | Miss     |
| ------------------- | ----------------- | -------------- | ---------------- | ------------ | --------------- | -------- |
| Air Up              | -166.67 < -83.33  | -83.33 < 0     | 0 < 200          | 200 < 283.33 | 283.33 < 366.67 | > 366.67 |
| Air Up with Tap     | -166.67 < -83.33  | -83.33 < 0     | 0 < 150          | 150 < 233.33 | 233.33 < 316.67 | > 316.67 |
| Air Down            | -266.67 < -183.33 | -183.33 < -100 | -100 < 150       | 150 < 233.33 | 233.33 < 316.67 | > 316.67 |
| Air Down with Tap   | -266.67 < -183.33 | -183.33 < -100 | -100 < 100       | 100 < 183.33 | 183.33 < 266.67 | > 266.67 |
| Air Action          | -266.67 < -183.33 | -183.33 < -100 | -100 < 100       | 100 < 183.33 | 183.33 < 266.67 | > 266.67 |
| Air Crush           | N/A               | N/A            | -266.67 < 266.67 | N/A          | N/A             | > 266.67 |
| Air Hold/Slide Tick | -600 < -400       | -400 < -200    | -200 < 0         | N/A          | N/A             | < -600   |

Air notes are slightly different from the other note types, notably having different windows for fast and late judgements. Air Up/Down with taps are slightly stricter than their variants without taps.

_Note: starting in Chunithm NEW and above, there is an even more precise timing window within Justice Critical called ‘Justice Heaven'. These appear as the center column in the score distribution nomogram but do not affect gameplay or scoring in any way. They can be thought of as the equivalent of S-Crit in SDVX._
