# What is Ergodicity Economics?

## The Core Question

Ergodicity economics starts with a simple question that has profound consequences: Is the average outcome of many people doing something once the same as the average outcome of one person doing something many times?

Ensemble Average: The average outcome of many people in parallel (e.g., 1,000 people flip a coin once). This is like looking at a "snapshot" across a population.

Time Average: The average outcome for a single person over time (e.g., one person flips a coin 1,000 times). This is like looking at a "movie" of one person's life.

Traditional economics often assumes these two averages are the same. This assumption is called the ergodic hypothesis.

Ergodicity economics argues that for key economic measures, especially wealth, this assumption is wrong. Wealth is non-ergodic.

## The Model: A Deceptively "Good" Gamble

The Gamble: You have $100. You are offered a bet:
- 50% chance to win 50% of your wealth (wealth is multiplied by 1.5)
- 50% chance to lose 40% of your wealth (wealth is multiplied by 0.6)

### 1. The Traditional "Ensemble" View

Traditional economics asks: "What is the expected value of this gamble?"

This is an ensemble question. It's like imagining 1,000 "parallel yous" all taking the bet once.

- 500 of them win: $100 * 1.5 = $150
- 500 of them lose: $100 * 0.6 = $60

The average wealth of the group is: (500 * $150 + 500 * $60) / 1000 = $105.

Conclusion: The expected value is positive (+$5). A "rational" person should take this bet!

Even though the distribution is wide, the average (the red line) is clearly above $100.

### 2. The Ergodic "Time" View

Ergodicity economics asks: "What happens to me if I take this bet repeatedly over time?"

This is a time question. You don't have 1,000 parallel lives. You have one life that unfolds through time.

Let's see what happens if you play twice and get one of each outcome (which is the most likely long-term average)

- :Start: $100
- Play 1 (Win): $100 * 1.5 = $150
- Play 2 (Lose): $150 * 0.6 = $90

You are poorer than when you started! The order doesn't matter

- :Start: $100
- Play 1 (Lose): $100 * 0.6 = $60
- Play 2 (Win): $60 * 1.5 = $90

Every time you get one win and one loss, your wealth is multiplied by 1.5 * 0.6 = 0.9. You lose 10% of your wealth.

Conclusion: This is a terrible bet! If you play it repeatedly, you are almost mathematically guaranteed to go broke. The second plot in the model shows this clearly: the single player's wealth trends directly towards zero. The log-scale plot shows this decline as a straight line, which highlights the constant rate of decay.

## Why the Difference? (Additive vs. Multiplicative)

This is the entire crux of the argument.

Ensemble averages are additive. We added up the wealth of all 1,000 players: ($150 + $150 + ... + $60 + $60).

Time averages for wealth are multiplicative. Your wealth multiplies over time: Wealth_final = $100 * (multiplier_1) * (multiplier_2) * ...

You cannot use an additive tool (ensemble average) to evaluate a multiplicative process (time average).

### The Correct Tool: Log-Utility

So how should we evaluate the gamble from the time perspective? We need a tool that turns multiplication into addition. That tool is the logarithm (since log(A * B) = log(A) + log(B)).

Instead of calculating the expected wealth, we should calculate the expected change in log-wealth.

- Expected Log-Change: 0.5 * log(1.5) + 0.5 * log(0.6)
- 0.5 * (0.405) + 0.5 * (-0.511)
- 0.2025 - 0.2555 = -0.053

The expected change in your log-wealth is negative. This number, -0.053, is the growth rate of your wealth. This calculation correctly predicts that you will lose money over time and that you should REJECT the bet.

This idea is closely related to the Kelly Criterion in betting, which is a formula for sizing bets to maximize the long-term log-growth of capital, not the short-term expected value.
