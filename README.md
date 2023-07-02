# Connect4
Artificial Intelligence Connect 4 Player

## Commands to run:
| Command | Description | Datatype | Example | Default |
| ----------- | ----------- | ----------- | ----------- | ----------- |
| -p1 | Agent who will be acting as player 1. Name of agent eg minimaxAI | String | -p1 minimaxAI or -p1 monteCarloAI | human |
| -p2 | Agent who will be acting as player 2. Name of agent eg minimaxAI | String | -p2 minimaxAI or -p2 monteCarloAI | human |
| -seed| Seed for AI’s with stochastic elements | int | -seed 0 | 0 |
| -w | Rows of Gameboard | int | -w 6 | 6 |
| -l | Columns of Gameboard | int | -l 7 | 7 |
| -visualize | Bool to use or not use GUI | bool | -visualize True or - visualize False | True |
| -verbose | Sends move-by-move game history to shell | bool | -verbose True or -verbose False | False |
| -limit_players | Which agents should have time limits. Useful if you want to play an AI but don’t want to have the same time limit. In the format “x,y” where x and y are players. Values that are not 1 or 2 can be used in place of 1 or 2 if the player should not be limited | String | -limit_players 1,2 or -limit_players -1,2 or -limit_players 1,-1 | 1 or 2 |
| -time_limit | Time limit for each player. No effect if a player is not limited. In the format “x,y” where x and y are floating point numbers. | String | -time_limit 0.5,0.5 | 0.5, 0.5 |

## Example commands:
  * python main.py -p1 minimaxAI -p2 stupidAI -limit_players 1,2 -visualize False -verbose True -seed 0
  * python main.py -p1 monteCarloAI -p2 minimaxAI -limit_players 1,2 -visualize False -verbose True -seed 0
  * python main.py -p2 alphaBetaAI -limit_players 2 -visualize True -verbose True
