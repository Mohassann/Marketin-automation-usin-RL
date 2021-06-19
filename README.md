# Marketing-automation-using-RL

In the marketing literature, learning consumers’ preferences from observed behavior is a controversial issue. The decision-making, campaign analysis in dynamic environment are the main challenges brought by online businesses. Therefore, there should be a way that can lead to easier decision-making and understand user’s preferences in a better way. We explained different marketing activates and scenarios, also explained whether Reinforcement Learning (RL) can be applied to those scenarios or not. We showed email marketing as an RL problem using contextual bandits. We implemented different exploration algorithms to achieve the highest click-through rate (CTR). Later we implemented a simple supervised learning algorithm. Our results show RL would largely outperform the supervised learning in email marketing campaigns. 

***
we used [VW library](https://vowpalwabbit.org/tutorials/contextual_bandit)


## Data format

| User's Gender | Time of the day  | Title 1 | Title 2 | Title 3 | Title 4 |
| ------- |:-------:|:---------------:| ----------|----- |----- |
| ------- | ------- | --------------- | ----------|----- |----- |
| ------- | ------- | --------------- | ----------|----- |----- |


***

## vowpal_wabbit Command lines

- **-q** :  [ --quadratic ] arg   Create and use quadratic features
- **--quiet** : Don't output diagnostics
- **--cb** : The contextual bandit module which allows you to optimize predictor based on already collected data, or contextual bandits without exploration.

- **--cb_explore** : The contextual bandit learning algorithm for when the maximum number of actions is known ahead of time and semantics of actions stays the same across examples.

- **--cb_explore_adf** : The contextual bandit learning algorithm for when the set of actions changes over time or you have rich information for each action. Vowpal Wabbit offers different input formats for contextual bandits.

**Note** that unlike ***--cb_explore***, we do not specify the number of actions in ***--cb_explore_adf*** as they are inferred from the number of lines in each example


***

## Exploration algorithms
1. **Explore-First**
2. **Epsilon-Greedy**
3. **Bagging explorer**
4. **Softmax Explorer**

***
## Exploration algorithms and their parameter’s values

| ------- | Explore-First | Epsilon-Greedy | Bagging | Softmax |
| Values | 2 | 0.1 & 0.2 | 3 | Lambda 10 |

