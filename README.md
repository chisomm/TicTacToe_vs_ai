# TicTacToe_vs_ai
This is an implementation of a program that a human play a game of Tic Tac Toe against a computer with 2 levels

# Inspiration from https://geekflare.com and https://www.thecrazyprogrammer.com
# There is a computer player in that will either make random moves (easy) or strategic moves to win (hard)

# Algorithm:

# 1. Create a board by initialising a 2d array with each elm initialised as '-'

# 2. Write a function to check whether the board is filled or not
  # iterate over the board and return False if any elm in 2d list is '-' else True

# 3. Write a function to check whether a player has won or not
  # check all 8 possible winning arrangements: all 3 rows, all 3 cols and both 2 diagonals

# 4. Write a function to show the board becuse it will be displayed throught game

# 5. Write a function to implement random computer move
  # find random number between 1 and 9 inclusive => generate loc
  # while loc is not in empty space list regenerate loc
  # once found empty loc then map to board idx and put sign there

# 6. Write a function to implement ai computer move
  # check if next move is winning for computer 
    # check if putting sign in any empty spaces makes has_player_won function True for computer sign
    # reset each time
    # if True then return that space for computer to play
  # check if next move is winning for opponent
    # check if putting sign in any empty spaces makes has_player_won function True for opponent sign 
    # reset each time
    # if True then return that space for computer to play
  # check if any of empty spaces is in corners set
  # check if any of empty spaces is in centre set
  # check if any of empty spaces is in sides set

# 7. Write function to start the game
  # Select the first turn of the player randomly
  # Write infinite loop that breaks when game over (win or draw)
    # Show board to user to select spot of next move
    # Ask the user to enter square number
    # update spot to respective player sign
    # check whether currnet player has won game or not
    # if player has won game: print winning message (output of the game) and break infinite loop
    # check whether board is filled or not (this line will run if curr player did not win game)
    # if board is filled: print draw message (output of the game) and break the infite loop
  # show the user the final view of the board
