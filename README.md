# Git tic-tac-toe

📚🎓 Learn to use GitHub pull requests and solve merge conflicts 😐 by playing [tic-tac-toe ❎🅾️❎](https://en.wikipedia.org/wiki/Tic-tac-toe) via git [pull requests](https://docs.github.com/en/github/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests).

## Game board

Example of a valid state of the game after players have taken four turns:

```
     |     |
  X  |  -  |  -
_____|_____|_____
     |     |
  -  |  O  |  X
_____|_____|_____
     |     |
  -  |  O  |  -
     |     |
```


## How to play

### Preparation

1. All players join either team X or team O.
2. All players clone this repository - you should be in the `main` branch by default.

### First turn

1. Team X begins: Player 1 of team X creates a new branch (e.g. `git branch move-01`).
2. Player 1 sets an `X` somewhere, e.g. it changes `game-board.txt` to the following:

  ```
       |     |
    X  |  -  |  -
  _____|_____|_____
       |     |
    -  |  -  |  -
  _____|_____|_____
       |     |
    -  |  -  |  -
       |     |
  ```

3. Player 1 commits the change locally (e.g. `git commit "Ingenious move"`)
4. Player 1 pushes the new branch to the remote repository (`git push`) - git might ask you to first create the remote branch - the prompt will contain instructions to do so.
5. Inside GitHub Player 1 opens a pull request (a.k.a. **PR**) ("New pull request") from the newly created branch onto `main`.
6. Player 1 adds all other players (including the opponents) as reviewers to the **PR**.
7. If all reviewers approve the PR, player 1 merges the PR.

  - This step might not work right away. In case of merge conflicts, player 1 has to pull

### Other turns

- The game continues. Its Team O's turn. A player of Team 0 follows all the steps above (just uses `O` as a symbol).
- Teams take turns in this manner until we have a winner or a draw.
