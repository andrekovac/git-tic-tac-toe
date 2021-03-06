# Git tic-tac-toe

ππ Learn to use GitHub **pull requests** and solve **merge conflicts** π by playing [tic-tac-toe βπΎοΈβ](https://en.wikipedia.org/wiki/Tic-tac-toe) via git [pull requests](https://docs.github.com/en/github/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests).

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

1. Team X begins: Players of team X each create a new local branch (e.g. `git checkout -b move-01`).
2. Players of Team X set an `X` somewhere, e.g. it changes `game-board.txt` to the following for player 1:

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

3. Players of Team X commit their changes locally (e.g. `git commit "Ingenious move"`)
4. Players of Team X push the new branch to the remote repository (`git push`) - git might ask you to first create the remote branch - the prompt will contain the command to do so (probably `git push --set-upstream origin move-01`).
5. Inside GitHub players of Team X open a pull request (a.k.a. **PR**) ("New pull request") from the newly created branch onto `main`.
6. Each player adds all other players (including players of Team O) as reviewers to the **PR**.
7. If all reviewers approve the PR, player merges the PR.

  - This step might not work right away. In case of **merge conflicts**, players have to discuss in comments of PR and resolve merge conflicts.
  - To this end you'll have to pull changes from the remote server (`git pull`) and resolve the conflicts.

### Other turns

- The game continues. Its Team O's turn. All players of Team 0 follow the steps above (just uses `O` as a symbol).
- Teams take turns in this manner until we have a winner or end in a draw.
