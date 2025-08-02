# ajedrez-slot-stake
Chess-themed slot with interactive board bonus
# Chess Slot - Interactive Bonus Concept

## 🎯 Project Description

A chess-themed slot game featuring animated chess pieces as symbols (pawns, rooks, knights, queens, kings) and a unique interactive bonus mode.

The game combines the strategy and elegance of chess with the fast-paced excitement of a slot machine.

---

## 🎮 Core Gameplay

- Classic slot spins with chess piece symbols.
- Stylish animations and sound effects based on chess moves.
- Each piece has a distinct value and visual style.

---

## 🧠 Bonus Feature: "Master Moves"

```python
def activate_bonus():
    board = create_board(4, 4)  # 4x4 empty board
    moves = 3
    rewards = 0

    while moves > 0:
        piece = choose_piece()  # player selects a chess piece
        position = choose_position(board)  # player selects position on the board
        place_or_move_piece(board, piece, position)
        moves -= 1

    winning_lines = check_lines(board)
    rewards += calculate_rewards(winning_lines)
    return rewards
