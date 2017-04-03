See images/ folder for related screenshots

f_score: this is defined as the sum of the g_score and the h_score. The shortest
path involves following the path of the smallest f_score values.

g_score: This is the cumulative number of tiles from the starting position. So if
Paul goes right 2 squares, that tile has a g_score of 2. If he goes 3 tiles to
the right and 2 tiles down, that tile will have a g_score of 5 (assuming only vertical
and lateral motion).

h_score: This is the "manhattan" score based on the raw distance between
the current tile and the destination tile (cake!). This is calculated regardless
of lava or other obstacles.

Diagonal motion: In this case, Paul goes diagonally between the lava because the added
cost value of 3 cancels out because taking a detour using just lateral motion would take 10 + extra steps!

Hops: In this case, Paul could go all the way around, but the higher cost of hopping
over one lava block is largely outweighed by the cost of having the double all the way around and take a diagonal step in the bottom left corner!

Swamp: In this case, the added cost of going through a swamp is much less than
having to jump over the wall of lava!
