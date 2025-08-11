# Notes on things
I am fortunate enough to have learned a bunch of things. But sometimes I forget them. So I'm making a list of stuff I find cool 

## Econ

### Game theory

<details>
  <summary>ECON 159 Game Theory @ Yale by Ben Polak (2008)</summary>
    1. <a href="https://www.youtube.com/watch?v=nM3rTU927io&list=PL6EF60E1027E1A10B&index=1&ab_channel=YaleCourses">Lecture 1</a> 
    <br/>
    Takeaways:
    <br/>
      i. Similar to optimization, you need to know your objective function (payoffs) before doing any analysis. Perhaps you value something (e.g. comfort) over another thing (e.g. speed) and weight then 2.5 : 1. But game theory doesn't tell you what your payoffs are. 
      <br/>
      ii. If the payoff of strategy A strictly is always greater than the payoff of strategy B regardless of what others do then A strictly dominates B. Important to note A and B must be for same player, can't compare across players. Do not play a strictly dominated strategy.
      <br/>  
      iii. Rational choices can lead to inefficient outcomes. For example in Prisoner's Dilemma it is optimal for everyone to cooperate but it is rational to always defect. Always defecting leads to an inefficient outcome for everyone (e.g. wasting money on nuclear weapon development in an Arm's Race) but it is rational.
    <br/>
    2. <a href="https://www.youtube.com/watch?v=qQ3kFydI_xQ&list=PL6EF60E1027E1A10B&index=2&pp=iAQB">Lecture 2</a> 
    <br/>
    Takeaways:
    <br/>
      i. Formal definition of a game: set of players, set of strategies, payoff function. A play of the game (a strategy profile) is a strategy for each player. From there you can calculate the payoffs of each player for this strategy profile.
      <br/>
      ii. The key part of game theory is to analyze the game from the other players' shoes. They analyze the number picking game from last class. A common answer is 2/3 of 50 because they assume that others will guess randomly but others are not guessing randomly, they are trying to win. You have to be rational and also assume that others are rational, and know that others know that others are rational and so on. This is so-called "common knowledge" when it goes all the way down infinitely. People who guessed >67 are not rational. People who guess >45 and less than 67 are rational and do not assume others are rational. The higher power of 2/3 * 100 is what layer of knowledge they assumed about others. The average was 13.3 and 2/3 of that is 9. (2/3 ^ 6 * 100 ~= 8.8). Because some people didn't play rationally or didn't assume common knowledge, the average was higher than 1. Playing this game again after having learned about this analysis everyone chose a lower number than last time. Average ~= 5. Because you know how to play the game better and you know that everyone else knows it better too AND they know you are better at playing and so on...
      <br/>  
      iii. If strategy payoff of strategy A is always greater or equal to the payoff of strategy B, A weakly dominates B. Don't play weakly dominated strategies. 
      <br/>  
      iv. Ok one more takeaway. Common knowledge is quite subtle. It is different than mutual knowledge. Person A has a pink hat, can't see their own hat can see Person B has a pink hat. B can't see their own hat. It is mutual knowledge that there is at least 1 pink hat but not common knowledge. 
      <br/>
      2. <a href="https://www.youtube.com/watch?v=kqDu0RVWTYw&list=PL6EF60E1027E1A10B&index=3&ab_channel=YaleCourses">Lecture 3</a> 
      <br/>
      Takeaways:
      i. Median voter theorem
</details>

**Summary:** [Link](https://www.youtube.com/watch?v=nM3rTU927io&list=PL6EF60E1027E1A10B&ab_channel=YaleCourses). First game theory course aimed at undergrads. Overall a good mix of math and anecdotes & games. Plays games in class often. Game Theory is about economic environments where there are multiple players trying their best to maximize their utility. This makes the game not-static and often harder to analyze becuase the other player may update their strategy in response to yours which may cause a change in yours and so on. 

**Three big takeaways**

1. There are common games (e.g. Prisoner's Dilemma, Battle of the Sexes, Rock Paper Scissors etc. [full list here](https://en.wikipedia.org/wiki/List_of_games_in_game_theory)) and most games can be reduced to one of these. Then you can use analysis from those games to analyze your situation. For example: this arm's race is a version of Prisoner's Dilemma. This is a super useful tool, leverage work done by very smart people. My favorite example is cleaning your room with your roommate. You really don't want to clean up your roommate's mess, but if neither of you clean it's bad but better than cleaning if your roommate doesn't. Note that this can be avoided by explicit cooperation (e.g. a contract with your roommate about cleaning, note that the contract effectively changes the payoffs because breaking it has consequences). Repeatedly playing this game will change the optimal strategy as well. Games can differ in payoffs, number of rounds, coordination, communication, imperfect information, asymmetric information, probabilistic games etc. 
2. Another reduction technique is called "iterative deletion" where you can remove strategies that are strictly worse (dominated) by another if their payoff is always worse than the other strategy regardless of what others do. It is iterative because once a strategy is removed we analyze the game again and we might be able to delete more strategies. We keep going until no more strategies can be deleted. For example a game where everyone guesses an integer between 1 & 100 and the payoff is abs(guess - 2/3 * average guess). Clearly 67 dominates every guess above 67 because if everyone guess 100, then 2/3 * average = 67 and the average is anything less than 100, 67 is always better. Now we can re-analyze the game where people can only guess between 1 & 67. 2/3 * 67 ~= 45 so we can delete everything above 45. We can keep doing this until we arrive at the only strategy being guessing 1. Note that before we deleted everything above 67, we couldn't delete everything above 45. That's a super important point! Doing this process iteratively gives you new information about the game. An important point about this game is that the first time people play it, they may play non-optimally and therefore the winning guess may be higher than 1! 
3. Some games require probabilistic or so-called mixed strategies. In rock paper scissors you randomly pick between all three because if you always picked one, your opponent would always pick the option that beats your option. In those games a Nash Equilibria exists and at that point you choose a strategy that makes your opponent indifferent towards the different options. (e.g. your opponent plays option 1 25%, option 2 75% and "players are indifferent between their available strategies because each strategy yields the same expected payoff"). What's interesting is that your strategy is determined by your opponent's payoffs. So if we change option 1 to be 10x more payoff for you, it doesn't change your strategy at equilibrium, it only changes your opponents!
