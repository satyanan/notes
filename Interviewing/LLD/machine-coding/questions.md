- Implement a thread-safe data structure which can keep track of number of incoming
requests grouped by IP Address over a time window. Add support for grouping by other
attributes such as BrowserAgent.
- Implement a thread-safe data structure which implements a leaderboard in game with following methods [solution](https://www.webonise.com/this-is-how-we-improved-players-rank-and-leaderboard-calculations-in-trivia-apps/)
  - getRankOfPlayer(player)
  - getPlayerAtRank(rank)
  - getScoreboardForPlayer(player)
    - this can use getRankOfPlayer(player) and then use the rank to get players around the same rank+-5
- Design APIs 