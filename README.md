# Russian-Roulette-Simulation
A simple Python simulation of a Russian Roulette game between 2 players. There are 4 simulation in total.


## The first simulation:
**1 loaded chamber and the cylinder is re-spun every turn**

The code provided runs a Russian Roulette Simulation for 2 players (A and B). The code has the function simulation(num, gameTotal) which is used to run the simulation in total of 'num' times (captured from input) and each simulation has 'gameTotal' = 100000 games. In each game, a counter starting from 1 will be initialized and a number in the set {0,1,2,3,4,5} will be randomized. If the random number is not 0, which has the probability of 5/6, the counter will increase by 1 and a new number will be randomized. Only until 0 is randomized, the game will be stopped and the loser will be determined by the parity of the counter (Player A will lose if the counter is odd and vice versa). 


## The second simulation:
**2 adjacent loaded chambers and the cylinder is re-spun every turn**

The function simulation(num, gameTotal) is changed into simulation2(num, gameTotal) with 0 and 1 are the two numbers used to determine when the one of the two loaded chamber is triggered. The odds of one of the two numbers being randomized are 2/6 (33.33%).


## The third simulation:
**2 adjacent loaded chambers and the cylinder NOT is re-spun every turn**

The function is one more time changed into simulation3(num, gameTotal) with 2 adjacent randomized numbers for the two loaded chambers (if the first number is 5 then the second number will be 0). A new number, the starting chamber, is randomized, and this number increases by 1 every turn. If this number gets to 5, the last chamber, and the game still doesn't end, the number is looped back to 0.


## The fourth simulation: 
**2 random loaded chambers and the cylinder NOT is re-spun every turn**

The function simulation3(num, gameTotal) is changed into simulation4(num, gameTotal) with a little tweak this time. Instead of 2 adjacent randomized numbers, this time 2 different numbers are chosen to be the 2 loaded chambers.
