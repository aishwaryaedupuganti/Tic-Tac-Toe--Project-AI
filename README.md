<b><H1>Tic-Tac-Toe game implementation</H1></b>
















![image](https://github.com/aishwaryaedupuganti/Tic-Tac-Toe--Project-AI/assets/78846108/84f6a690-7789-44d7-9678-8ffdb1fa1489)


<b><H1>Introduction</H1></b>

Tic-tac-toe is a two-player game played on a 3x3 grid. One player plays as "X" and the other player plays as "O". Players take turns placing their symbol in an empty square of the grid. The objective of the game is to get three of your symbols in a row, either horizontally, vertically, or diagonally. The first player to get three in a row wins the game. If all squares are filled and no player has three in a row, the game is a tie.


<b><H1>Implementation</H1></b>

We are combining algorithms such as the Min-Max algorithm, Alpha-Beta pruning, and Q-learning in this project. The Min-Max algorithm generates a decision tree that represents all possible moves and outcomes. The decision tree can then be pruned using alpha-beta pruning to remove branches that are unlikely to lead to a winning move. Finally, Q-learning can be used to improve AI agent performance by allowing them to learn from their past experiences.


![image](https://github.com/aishwaryaedupuganti/Tic-Tac-Toe--Project-AI/assets/78846108/463c795a-fdee-4929-a7cf-892ef035a6be)

The AI agents would compete against each other in this implementation. To make decisions, one agent would employ the Min-Max algorithm with Alpha-Beta pruning. Another agent would make decisions based on Q-learning. The two agents would play a variety of games, with the Q-learning agent learning from its previous experiences to improve its performance over time.

<b><H1>Objective</H1></b>

The goal of this project is to create an intelligent system that can play Tic Tac Toe at a high level by designing an adversarial search algorithm and reinforcement agents. The AI agents would learn from their previous experiences and improve their performance over time, resulting in a more difficult and engaging game.

Three Artificial Intelligence Agents were created:

 1.Q Learning Method
 
 2.The Min-Max Algorithm

 3. Pruning Alpha-Beta

To find the most efficient Algorithm, play Tic Tac Toe with them several times. Comparing the efficiency of three algorithms by calculating the corresponding performance metrics and determining which algorithm performs better, adversarial search or Reinforcement Learning. Finally, the main goal of this project would be to develop an intelligent system capable of learning and adapting to new challenges, resulting in more robust and capable AI systems in the future.

<b><H1>Approaches</H1></b>

The first step is to put Q-Learning from Reinforcement Learning into action.

The following step is Adversarial Search, which employs the two algorithms listed below.

       1. The Min-Max Algorithm
       
       2.Alpha-Beta Pruning. 

Technology Stack: 1.Python

![image](https://github.com/aishwaryaedupuganti/Tic-Tac-Toe--Project-AI/assets/78846108/645901cf-bd09-49e7-95d2-31d491d6482c)

<b><H1>Brief Description of AI</H1><b>

<b><H1>Min-Max Algorithm</H1></b>

The Min-Max algorithm in Tic-Tac-Toe works by first creating a decision tree that represents all possible moves and outcomes, and then recursively evaluating each possible move to determine which one leads to the best outcome for the player.

The algorithm alternates between maximizing and minimizing the game's outcome at each level of the decision tree. For example, if the algorithm is attempting to find the best move for the "X" player, it will maximize the game outcome at each level, assuming that the "O" player will make the best possible move.
Each outcome is given a score by the algorithm, with a higher score indicating a better outcome for the "X" player and a lower score indicating a better outcome for the "O" player. The algorithm then chooses the move that gives the "X" player the highest score or the lowest score for the "O" player.
The algorithm in Tic-Tac-Toe can evaluate all possible moves on the 3x3 grid to determine the best move to make. However, as the game becomes more complex, so does the number of possible moves, making it difficult for the algorithm to evaluate all possible moves in a reasonable amount of time. That's where techniques like Alpha-Beta pruning and Q-learning come in to help narrow the search space and improve the algorithm's efficiency.

![image](https://github.com/aishwaryaedupuganti/Tic-Tac-Toe--Project-AI/assets/78846108/8662d268-70eb-4f48-97ea-00ba7a72ce07)

<b><H1>Alpha-Beta</H1></b>
In Tic-Tac-Toe, Alpha-Beta pruning works by removing decision tree branches that are unlikely to lead to a better outcome.
During the Min-Max algorithm, Alpha-Beta pruning keeps two values, alpha and beta, which represent the best possible score for the maximizer (e.g. "X" player) and the best possible score for the minimizer (e.g. "O" player), respectively. As the algorithm evaluates each node, it updates these values and prunes any nodes that will not result in a better outcome than the nodes that have already been evaluated.
Assume the algorithm is evaluating a node where the maximizer (e.g. "X" player) has already found a move that results in a score of 2 and is evaluating a child node that can only result in a score of 1 or less. Because the minimizer (for example, "O" player) will never choose a move that results in a score of 1 or less, the algorithm can prune that branch of the decision tree and proceed to evaluate other nodes.
In Tic-Tac-Toe, Alpha-Beta pruning can significantly reduce the number of nodes that must be evaluated, especially when the game's outcome is clear. By narrowing the search space, the algorithm can more efficiently use its computational resources to find the best move.

![image](https://github.com/aishwaryaedupuganti/Tic-Tac-Toe--Project-AI/assets/78846108/fa25b1f5-5ef6-4083-96c0-6c2057195594)

<b><H1>Q-Learning</H1></b>
Q-learning is a reinforcement learning algorithm that can be used to teach an artificial intelligence agent how to play Tic-Tac-Toe. The AI agent learns in Q-learning by playing multiple games and observing the outcomes of its actions. After that, the agent updates its "Q-table," which contains values representing the expected reward for each action in each state of the game.
The Q-table begins with random values, but as the agent plays more games, the values in the table are updated based on the rewards it receives. For example, if the agent makes a move that results in a win, the Q-table will be updated to increase the expected reward for that move in that state of the game. If the agent makes a move that results in a loss, the expected reward for that move in that state of the game will be reduced. The AI agent learns which moves are more likely to result in a win or a loss over time and adjusts its behavior accordingly. The AI agent can improve its performance and become a more difficult opponent by continuously updating the Q-table based on its experiences.
The AI agent in Tic-Tac-Toe can use the Q-table to determine which move to make in each state of the game. According to the Q-table, the agent will select the move with the highest expected reward in that state. The Q-table is updated with better estimates of the expected rewards as the agent plays more games, and the agent's performance improves.


![image](https://github.com/aishwaryaedupuganti/Tic-Tac-Toe--Project-AI/assets/78846108/1aa9c300-cf3e-4adc-aa15-5812106d2751)

<b><H1>Deliverables</H1></b>
a.User Documentation Model, which provides information about the implementation of the Tic Tac Toe game using Min-Max, Alpha-Beta, and Reinforcement Learning Agents.

b.Algorithms written in Python for use with AI Agents (.py files)

c.A link to the Python code and related files on Github.

d.A YouTube video demonstrating the project and its implementation through the use of slides.

<b><H1>Evaluation Methodology</H1></b>
When evaluating the performance of AI agents playing Tic-Tac-Toe, several metrics can be used to determine their effectiveness.
Win rate: The percentage of games won by the AI agent against a specific opponent. The better the agent's performance, the higher the win rate.
Average number of moves per game: The average number of moves made by the AI agent to win or lose a game. A lower average number of moves indicates that the agent is more efficient and strategic in his or her movements.
Training time: This is how long it takes the AI agent to learn how to play Tic-Tac-Toe. A shorter training time indicates that the agent is learning faster and more efficiently.
Performance against various opponents: It is critical to test the AI agent's performance against various opponents of varying skill levels. This determines how well the agent adapts to different playing styles and skill levels.
Human-like behavior: A good AI agent should be able to not only win games but also exhibit human-like behavior, such as making moves that are not only aimed at winning but also at blocking the opponent's moves.










