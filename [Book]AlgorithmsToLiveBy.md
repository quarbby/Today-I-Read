### Algorithms To Live By

Brian Christian & Tom Griffin
[Link](https://www.amazon.com/Algorithms-Live-Computer-Science-Decisions/dp/1627790365)

Thirty-seven percent: If you want the best odds of getting the best apartment, spend 37% of your apartment hunt noncomittally exploring options. Leave the checkbook at home; you're just calibrating. But after that point, be prepared to immediately commit -- deposit and all -- to the very first place you see that beats whatever you've already seen. This is a provably optimal solution, "optimal stopping" problem

In any optimal stopping problem, the crucial dilemma is not which option to pick, but how many options to consider. 

Optimal solution takes the form of what we'll call Look-Then-Leap Rule: You set a predetermined amount of time for "looking" -- exploring your options, gathering data -- in which you categorically don't choose any one, no matter how impressive. After that point, you prepare to instantly commit to anyone who outshines the best applicant you saw in the look phase.

The irrestible question is whether -- by evolution or education or institution -- we actually do follow best strategies. People tend to stop early, leaving better applicants unseen.
BEcause for people there's always a time cost. It doesn't come from the design of the experiment. It comes from people's lives.

Everyday we're constantly forced to make decisions between options that differ in a very specific dimension: do we try new things or stick with our favourite ones? We intuitively understand that life is a balance between novelty and tradition, between the latest and the greatest, between taking risks and savouring what we know and love. 


Explore vs Exploit

Exploration is gathering information, and exploitation is using the information you have to get a good known result.

Multi-armed bandit problem

People tend to treat things in isolation, to focus on finding each time the outcome with the highest expected value.
The value of exploration, of finding a new favourite, can only go down over time, as the remaining opportunities to savour it dwindle. The flip side is that the value of exploitation can only go up over time. 

Win-Stay, Lose-Shift algorithm: choose an arm at random and keep pulling it as long as it keeps paying off. If the arm doesnt pay off after a particular pull, choose another one.

Regret is the result of comparing what we actually did with what would have been best in hindsight. In a multi-armed bandit, Barnad's "inestimatable loss" can in fact be measured precisely, and regret assigned a number: its the difference between the total payoff obtained by following a particular strategy and the total payoff that theoretically could have been obtained by just pulling the best arm every single time.

Mathematician Tze Leung Lai were able to prove several key points about regret. First, assuming you're not omniscient, your total amount of regret will probably never stop increasing, even if you pick the best possible strategy -- because even the best strategy isn't perfect every time. Second, regret will increase at a slower rate if you pick the best strategy than if you pick others.
