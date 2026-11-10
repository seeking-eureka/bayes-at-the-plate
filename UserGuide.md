# Bayes at the Plate: A Plain-English Guide

## The Big Idea

A batter's **batting average** is hits divided by at-bats. A .300 hitter gets a hit about 3 times in every 10 at-bats. Over a full 160-game season, that's very good.

Here's the puzzle. Two weeks into the season, our batter is hitting .350. Is he suddenly a superstar, or is he on a lucky streak? Fans tend to believe the hot start. Scouts tend to believe the player's track record. The truth is usually somewhere in between.

This app shows how to find that "in between" using a rule called **Bayes' Theorem**. The rule is simple: start with what you already know, then adjust as new evidence comes in. Adjust a little when the evidence is thin, and a lot when it's strong.

## How the App Thinks

1. **Start with history.** Our batter hit .280 two seasons ago and .288 last season. The app blends those into a starting belief: he's about a **.285 hitter**. Last season counts a little more because it's more recent.
2. **Add new evidence.** Every 10 games, the app adds this season's hits and at-bats to the record.
3. **Forecast the finish.** It predicts his batting average at the end of the season and gives a range of likely outcomes.

Early in the season, history does most of the work. By late in the season, this year's results take over. Nobody has to decide when to switch. The math handles it automatically, based on how much evidence there is.

## Reading the Screen

The Simulator tab has a few main parts.

- **The slider.** Move it to any point in the season, or press Play to watch the season unfold 10 games at a time.
- **10-game average.** How he hit in the latest stretch. This number jumps around a lot.
- **Season average.** All of his hits and at-bats so far.
- **Bayes final.** The app's forecast of where his average will finish, with a 95% range. "95% range .278–.343" means the app is quite confident he'll end up between those two numbers.
- **True talent.** The app's best guess at how good a hitter he really is, with luck stripped out.
- **Uncertainty curve.** Each bar is one possible final average. Taller bars are more likely. As the season goes on, the curve gets narrower because there's less left to guess.
- **Game log.** Every 10-game stretch is listed, and you can edit any of them.

## A Season in Four Moments

The sample season is worth walking through.

**Opening day.** There's no data yet, so the forecast is just his history: **.285**, with a range of .229 to .343. That's wide because a whole season of luck is still ahead.

**Game 20.** He's hitting **.350**. The app's forecast moves up, but only to **.300**. Twenty games aren't enough to throw out two seasons of history.

**Game 80.** He's still hitting well, at **.322**. Now the forecast is **.310**, and the range has narrowed to .278 to .343. The evidence is stronger, so the app trusts it more.

**Game 160.** He finishes at **.323**, a career year. But the app's "true talent" estimate is only **.305**. One great season makes him look better, but not quite as good as his final number. Some of that season was probably luck.

## Why This Matters Beyond Baseball

Board members face the same puzzle all the time. A new vendor has a perfect first quarter. A new fund manager beats the market for six months. A control passes its first audit. Each is a hot start. The Bayesian question is always the same: **how much should this new evidence change what we believed before?**

The app teaches three habits:

- **Small samples are noisy.** A great two weeks, or a great quarter, proves less than it seems to.
- **History matters, but it shouldn't win forever.** Strong, sustained evidence should change your mind.
- **Always ask for the range, not just the number.** A forecast of ".310" means little without knowing whether the range is narrow or wide.

## Things to Try

- Press Play and watch the forecast start out cautious and then catch up with his hot start.
- Give him one terrible 10-game stretch early in the season, then one late in the season. Notice which one moves the forecast more.
- Click the weights line under the two past seasons and choose "Pooled 1.0 / 1.0." Trusting history more heavily makes the forecast slower to react.

## Limits to Keep in Mind

- **The player isn't real.** The batter and his seasons are made up for teaching.
- **Real forecasting systems use more information,** such as age, injuries, and ballpark. This app keeps things simple so the logic is easy to see.
- **A forecast isn't a promise.** It describes what's likely, not what's certain.
