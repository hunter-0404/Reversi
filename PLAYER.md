## The Player

The pieceColor would be able to interact with the model in one of two ways.
- For starters, they could merely pass their turn. This would immediately end their turn, without
placing a piece on the board. This would be useful if they have no valid moves, or if they want to
end the game early. If both players pass their turn in a row, the game is considered over.
- Alternatively, the pieceColor could play a move on the board, passing in X- and Y- coordinates 
corresponding to the move they want to play. If the move is determined to be valid, that spot will 
be filled with the pieceColor's piece, and all the surrounding pieces that were the other pieceColor's
color. Otherwise, the pieceColor will be notified that their move was as such, and should be prompted 
to try again. 

## AI
If we wanted to, we could allow an AI to act as the other pieceColor, turning it from a two-pieceColor game
into a single-pieceColor game. This would be done by having the AI play a move after the pieceColor plays
a move. The AI would be able to determine the best move to play by calculating which move would 
result in the most pieces being flipped to its color, and playing that move. 