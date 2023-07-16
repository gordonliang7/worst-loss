# worst-loss
This notebook explores using pandas's groupby().apply() method chain to scan through MLB games and determine which loss was a team's worst loss within the data.

DISCLAIMER: The data is comprised of 5% of wins and 5% of losses for each AL West Team. As a result of the data not being complete,
  the results you find here are not necessarily representative of the actual results. (For example, if World Series Game 1 isn't in
  the sample, you're not going to have the actual worst loss for the Houston Astros but only the worst loss within that 5% included).

CHECK YOUR UNDERSTANDING ANSWERS:
1. This will return a team's best comeback win within the sample
2. All three functions reference gameDF which isn't defined in the global scope so if we
   define it in the global scope, we'll get an error upon calling. By nesting the helper function,
   calling it will result in it searching the scope of gameResult after being unable to find it in
   it's own scope. Additionally for homeWon and awayWon, returnedSeries is also not globally defined.
3. Whether the home team winning or the away team winning doesn't change the date of the game so adding
   it outside removes a line of us repeating ourselves.
