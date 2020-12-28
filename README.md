Full instruction to my work below:
clone this repository:
My advice is to download and extract it on PC;
Then Open it, (better to open it from intellij Idea) then you must be able to run, but first, I'll give you some information:
1) There are src, out, .idea. and (.iml, .in, .out) files in my folder
gamsrv.out file should contain the result.
this program uses a custom (dijkstra) algorithm to solve GAMSRV (that is given in lines below). gamsrv.in file is for input; it contains M+2 lines

I prefer using Dijkstra's algorithm to get the shortest path to each node, the program finds the Server location that minimizes the largest latency value to the Client, and prints this latency.

the algorithm works like this:

get the total number of nodes, number of client nodes, and edges from gamsrv.in file,
for each router, get latencies from it to all the clients,
find the max latency between the router and all the clients,
if the max latency is minimal, this router can be considered a good position for the server,
repeat 2-4 until there is no node left to calculate,
write the minimal max latency to gamsrv.out.
