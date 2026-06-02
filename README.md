# TicTacToe
 Digital Logic Design Implementation
A fully hardware-based implementation of the classic Tic-Tac-Toe game using D flip-flops, logic gates, bi-color LEDs, and push-buttons alon with win of three counter and display. No microcontroller or software  pure digital logic. Designed and simulated in Proteus Design Suite.

How It Works
Two players take turns pressing buttons on a 3×3 grid. Player X's moves light up blue, Player O's light up red. The circuit automatically tracks turns, detects a winner, and locks all inputs the moment the game ends.

<img width="718" height="665" alt="image" src="https://github.com/user-attachments/assets/485245a8-03ee-46d8-b06d-0bf6ad6f5b56" />

<img width="646" height="428" alt="image" src="https://github.com/user-attachments/assets/4f5b8b8a-d9c7-4efc-be6c-b9115a964fd0" />
Input Block Circuit

<img width="640" height="437" alt="image" src="https://github.com/user-attachments/assets/3c1c052b-97bd-4b0b-8a4b-fd036a4ff367" />
Single Push-Button Cell

<img width="622" height="512" alt="image" src="https://github.com/user-attachments/assets/e0d2d9f6-ba4a-412f-be2c-1d23e38c4c1e" />
Xor gate Block

<img width="657" height="345" alt="image" src="https://github.com/user-attachments/assets/33014898-6f3f-4994-972b-2762a1481e96" />
Control Block Circuit

<img width="632" height="491" alt="image" src="https://github.com/user-attachments/assets/7539ada1-a38c-43d5-a73b-63a4b3a357c3" />
Terminator Block

<img width="617" height="377" alt="image" src="https://github.com/user-attachments/assets/ad882cd7-ab83-42ec-8077-027813e7f2cc" />
Buttons Block

<img width="617" height="386" alt="image" src="https://github.com/user-attachments/assets/8f477bfe-7dfd-4a53-baf4-8a907f51e9d6" />
Output Block

<img width="622" height="165" alt="image" src="https://github.com/user-attachments/assets/d466f29a-d48b-4a6a-896c-97c6190cc39a" />
Reset Button Block

<img width="619" height="411" alt="image" src="https://github.com/user-attachments/assets/5690a6c7-ead2-4610-8013-8aa9dd1e6a52" />
Counter Block

Circuit Block
1.Input Block
9 push-buttons + D flip-flops (7474) to latch each player's move
2.XOR Gate Block 
Counts total moves via XOR parity to determine whose turn it is
3.Control Block 
Checks all 8 win conditions (3 rows, 3 columns, 2 diagonals) using AND/OR gates
4.Terminator Block
Freezes all inputs on win; lights green LED on draw 
5.3×3 LED Grid
Displays game state — blue for X, red for O
6.Counter with display
Counts and displays winner of three rounds

Key Features
Anti-cheat latch — re-pressing an occupied cell has no effect
Auto turn detection — XOR parity determines X or O without any counter IC
Win detection — all 8 conditions checked simultaneously in hardware
Draw indicator — green LED activates when all 9 cells fill with no winner
Master Reset — clears all flip-flops and restarts the game
Counter with display_Counts and displays winner of three rounds.

References
Design based on:
Aryaman Mihir Seth et al., "Implementation of Tic-Tac-Toe Game Using Digital Logic Design", IIT Bombay, March 2022
