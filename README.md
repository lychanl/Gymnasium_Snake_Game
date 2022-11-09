# Snake game for OpenAI Gym
![Python versions](https://img.shields.io/pypi/pyversions/gym-snake-game)
[![PyPI](https://img.shields.io/pypi/v/gym-snake-game)](https://pypi.org/project/gym-snake-game/)
[![License](https://img.shields.io/github/license/NaLooo/Gym_Snake_Game)](https://github.com/NaLooo/Gym_Snake_Game/blob/main/LICENSE)

 Snake game for OpenAI gym


## Quick Start
```python
import gym_snake_game
import gym

# both work
env = gym.make('Snake-v0', render_mode='human')
env = gym_snake_game.make('Snake-v0', render_mode='human')
env.reset()

# for human playing
env.play()

# for ai playing
while True:
    obs, reward, done, truncated, info = env.step(env.action_space.sample())
    if done:
        break
env.close()

```

**Ming Yu**