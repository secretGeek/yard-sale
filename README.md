# Yard-Sale-Model

This is a Web-based simulation of the 'Yard Sale Model' from physics/economics.

See it online here: **[Yard Sale Model Simulation](https://secretgeek.github.io/yard-sale/)**

After reading and enjoying this excellent article/simulation [Why the super rich are inevitable](https://pudding.cool/2022/12/yard-sale/) I wanted to tinker with the "Yard Sale Model" for myself.

## Description of the basic Yard Sale Model

1. Start with a population of people, all of whom have the same amount of money. (There are two constants to be set here: `populationSize` (e.g. `100`) and `moneyPerPlayer` (e.g. `$100`))
2. Pick 2 people at random to play a "heads/tails" betting game, with each person having the same chance of winning.
    - The amount they are betting on is a percentage of the poorer player's wealth. (Here we have another constant to set, `betPercent`). For example, if we choose "20%" as the max betting percentage, and the two players betting have wealth of $100 and $1 million dollars, then the "stakes" they are gambling for would be $20 -- 20% of the poorer player's wealth.
3. Repeat step 2 indefinitely. Keep an eye on what happens to the distribution of wealth amongst the population.

To begin with the distribution of wealth is perfectly "level" - everyone has the same amount of money. After one round of betting each player has either 1 loss or 1 win, so if they all started at $100, we now have  group where 50% of people have $80 and 50% have $120. This is called a "bimodal" distribution, two modes, the haves and the have nots.

As the rounds accumulate, you may expect people's wealth to bounce up and down around the $100 mark -- since the mean dollars per player is fixed (no money is being created or destroyed, no new players are joining, none are leaving.)

But what the Yard Sale Model instead shows is that, although an individual's wealth may bounce up and down from one bet to the next, people with less money are likely to continue to average toward less and less money, their money tending to accumulate in a group of "haves". And as time progresses forward, the group of "haves" tends to get smaller, until even 1 player captures close to $100 of all wealth.

The Yard Sale Model is used to demonstrate that wealth accumulation can arise naturally, even in a seemingly "fair" system, and without any variation in "skill" between players.

There are variants of the Yard Sale Model where extra factors are applied. For example, the application of a "tax" after each round, which moves each player some distance closer to the mean (i.e. "robbing the rich and giving to the poor") -- and its been shown that such models can, with the right factors, achieve a steady state with very similar wealth distribution to those observed in modern societies.

Critics of the Yard Sale Model indicate that "true" trades are not the same as these "zero-sum" gambles. For example, if I buy milk from a dairy farmer, I buy it because its value *to me* (thirsty for milk) is greater than the value it has for the farmer (who is not thirsty for milk) -- hence "value" is created in real trades.

## Variation with "non-zero sum" trades

One of the criticisms of the Yard-Sale Model is that it involves "zero-sum" trades. People like to claim that when value is created by the trades, the "magic hand" of the market somehow distributes the wealth more evenly.

I've built a variation of the simulation with "non-zero sum" trades.

It's quite difficult in practice to find a simple model that realistically depicts the "non-zero" nature of trades. Which trades are really non-zero? If i'm the final consumer of a product (e.g. milk, or cigarettes) then I'm not really gaining more than I've paid for a commodity, and I'm certainly not growing my wealth. Yet, the model shows that even if we pretended that both parties of a trade were gaining value in each trade, the gigantic wealth disparity still arises.

See the non-zero-sum variant here: **[Yard Sale Model Simulation](https://secretgeek.github.io/yard-sale/nonzero/)**


## More Variations

I'd like to explore so many variations of this!

Progressive taxation is the first thing I'd like to add. Done well, progressive taxation works wonder on this yard-sale model.

Then I'd like to add a "taxation under lobbying" variant. In this system there would, initially, be progressive taxation. But after every (say) 20 rounds there would also be the opportunity for each participant to "lobby" on how the tax model should change. Their lobbying position would align with their own self-interest (those below the median wealth would lobby for more progressive taxation, those above would lobby for less progressive taxation. And the catch is: the power of their lobbying depends on how much wealth they have.

I think this would show an illuminating model of how modern, "enlightened", democracies under capitalism work against themselves. In a democracy "votes" are power, but in capitalism, "wealth" is power. Can the two systems co-exist over time? Unless voters get an informed, equal, vote on *every* aspect of governance, capitalism steadily drives the intrinsic value of the vote itself toward zero. The model will show that, in the end, voting becomes a circus, the false dichotomy of choosing between near-identical figureheads selected by the oligarchy. Entertainment itself becomes the driving decider in the meaningless race.


## References

- [Why the super rich are inevitable](https://pudding.cool/2022/12/yard-sale/)
- [Is Inequality Inevitable? - Scientific American](https://www.scientificamerican.com/article/is-inequality-inevitable/)
  - [(PDF) Describing Realistic Wealth Distributions with the Extended Yard-Sale Model of Asset Exchange](https://www.researchgate.net/publication/301876072_Describing_Realistic_Wealth_Distributions_with_the_Extended_Yard-Sale_Model_of_Asset_Exchange)
- [Yard Sale Model - University of Maryland](http://www.physics.umd.edu/hep/drew/math_general/yard_sale.html)
- [Yard Sale Wealth Model - Hash.ai](https://hash.ai/@eadan/yard-sale-wealth-model)
- [Gini coefficient - Wikipedia](https://en.wikipedia.org/wiki/Gini_coefficient)
