# Tic-Tac-Toe-NNML

Tic Tac Toe Neural Network Machine Learning


This project provides a learning experiance from an AI that learns as it plays. The more games that you play, the further generations learn and play.

The AI is a Neural Network (NN) Cluster with 10 networks, each network takes in 9 points and gives 9 points. The Black Box in the network goes from 9 inputs to 9 nodes on the first layer, to 15 nodes on the second layer, and then 9 nodes as an output. The output is calculated by the greatest value of all the outputs. If an output is taken, then it will give the next highest output. The cluster of AI's at the end of the player's game finds the 4 highest scoring networks (score counts as games won during player game), and then creates 7 children for the next generation, another 1 child made from the top score network, and a completely random network to simulate variance between generations. The final two children are completely randomized, as to introduce even more varance between generations, and have potential to get over learning gaps that would otherwise not be possible. This is not a perfect representation of a genetic algorithm, but will represent the general concepts.

During the players game, each move made on their board, by the player and the AI, will cause a subgame in the background to be played between all NN. This subgame dictates if their score will increase or stay the same. The games are organized randomly, there are 5 teams, and each NN will be assigned a team, and each team member faces the other in a subgame. Once the player's game is finished, the scores from the subgames are tallied. 
