# Mars Crater Descent Simulation
Team:
Francisco Javier Chávez Ochoa A01641644
Miguel Emiliano González Gauna A01633816
Laura Merarí Valdivia Frausto A01641790
Overview:
This simulation explores the descent into a Martian crater using two optimization techniques:

Greedy Search: A heuristic method that makes the most promising choice at each step of the exploration.
Simulated Annealing: A probabilistic method that explores neighbors and can occasionally choose worse solutions to escape local optima.
Both techniques aim to find the lowest point in the crater based on elevation data.

Key Components:
Mars Map: A 2D elevation matrix representing the Martian terrain.
Crater Class: Represents the state of the explorer. Contains methods for calculating current elevation (cost) and finding neighboring points (neighbor).
Visualization: Uses plotly to visualize the path taken by each technique on the Martian map.
Simulation Flow:
Load the Martian terrain data.
Define the starting point.
Run the Greedy Search:
At each step, move to the neighboring point with the lowest elevation.
Continue until a specified number of steps or until no further descent is possible.
Run Simulated Annealing:
Start with an initial temperature and gradually decrease it.
Explore random neighbors. Accept neighbors based on cost difference and current temperature.
Continue until a threshold temperature or until no further descent is possible.
Visualize both paths on the Mars map using 3D visualization.
Results:
The results can be viewed as a 3D visualization in the generated 'mapa_marte.html' file. The paths taken by the Greedy Search and Simulated Annealing methods are shown in different colors.
