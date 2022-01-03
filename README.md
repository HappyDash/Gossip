# Gossip Simulator

GOSSIP SIMULATOR

Gossip type algorithms can be used both for group communication and for aggregate computation. The goal of this project is to determine the convergence of such algorithms through a simulator based on actors written in F#. Since actors in F# are fully asynchronous, the particular type of Gossip implemented is the so called Asynchronous Gossip.


The program prints the convergence time of all nodes for the following algorithms and topologies. For Gossip it ensures all nodes hear the rumour more than 10 times. For push-sum, all nodes' ratio of s/w should not have changed more than 10^-10 in 3 consecutive rounds.

HOW TO RUN:

Navigate to the folder with the file gossip.fsx

Run the following command on the terminal:

dotnet fsi proj2bf.fsx <numNodes> <topology> <algorithm>
Where numNodes is the number of actors involved (for 2D based topologies you can round up until you get a square), topology is one of full, 2D, line, imp3D, algorithm is one of gossip, push-sum.
