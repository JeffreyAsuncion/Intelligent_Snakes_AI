# Intelligent_Snakes_AI
Train an AI to Play Snake

# Project Outline
* Part 1 - Implement the game (environment)
* Part 2 - Implement the agent
* Part 3 - Implement the model


# Part 1 - Implement the game (environemnt)

### create virtual environment and install dependencies
* python3.7 -m venv pygame_env
* source pygame_env/bin/activate
* pip install pygame
* pip install torch torchvision
* pip install matplotlib ipython


# Part 2 - Implement the agent

* reset
* reward
	- Add reward to play(  ) and set to 0, -10, +10
* play(action) -->> direction
	- Remove the input from keyboard and pass in an action instead
	- Also returns the reward
    - Action
	    - [1, 0, 0] -->> straight
	    - [0, 1, 0] -->> right turn
	    - [0, 0, 1] -->> left turn
* game_iteration
* _is_collision
	- Check pt collision, if pt is None, self.head = pt
	- Replace self.head with pt
	- Is_collision should be public, so remove the prefix _ 
* move, direction -->> action
	- To determine that next move


*  remove the name == main driver code

* We will control this class from the agent,
* And call the play_step function


# Part 3 - Implement the model

* Rename to game.py
* And setup the agent

* We will use a deque to hold the moves

* Notes at video 44:10

* Def the init

* Def train

* get_state will take 


State (11 values)
[
 'danger straight', 'danger right', 'danger left',
 'direction left', 'direction right', 
 'direction up', 'direction down',
 'food left', 'food right',
 'food up', 'food down'
]

* remember

* train_short_memory

* train_long_memory

# Part Four

* implement model
* trainer
* plotting

