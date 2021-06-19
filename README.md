# Marketing-automation-using-RL

In the marketing literature, learning consumers’ preferences from observed behavior is a controversial issue. The decision-making, campaign analysis in dynamic environment are the main challenges brought by online businesses. Therefore, there should be a way that can lead to easier decision-making and understand user’s preferences in a better way. We explained different marketing activates and scenarios, also explained whether Reinforcement Learning (RL) can be applied to those scenarios or not. We showed email marketing as an RL problem using contextual bandits. We implemented different exploration algorithms to achieve the highest click-through rate (CTR). Later we implemented a simple supervised learning algorithm. Our results show RL would largely outperform the supervised learning in email marketing campaigns. 

***
we used [VW library](https://vowpalwabbit.org/tutorials/contextual_bandit)


## Data format

| User ID | Item ID | Rating (1 or 0) | Timestamp | Year | 
| ------- |:-------:|:---------------:| ----------|----- |
| ------- | ------- | --------------- | ----------|----- |
| ------- | ------- | --------------- | ----------|----- |

| Female  | :--------------: | :---------------: | ----------|----- |
| User    | Time of the day | Title 1 | Title 2 | Title 3 | Title 4 | 
| ------- | --------------  | --------------- | ----------|----- |
| Male    | --------------  | --------------- | ----------|----- |
| ------- | --------------  | --------------- | ----------|----- |


***
