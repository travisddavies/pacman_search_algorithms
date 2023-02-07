# Pacman Search Algorithms
This is based of UC Berkley's Intro to AI course. All code was provided by them except for the search algorithms and certain heuristic functions and search agents.
This was essentially to practice using informed and uninformed search algorithms used in AI. To play with various search functions, you can use the following commands:

## Depth First Search
```
python pacman.py -l tinyMaze -p SearchAgent
python pacman.py -l mediumMaze -p SearchAgent
python pacman.py -l bigMaze -z .5 -p SearchAgent
```

## Breadth First Search
```
python pacman.py -l mediumMaze -p SearchAgent -a fn=bfs
python pacman.py -l bigMaze -p SearchAgent -a fn=bfs -z .5
```

## Uniform Cost Search
```
python pacman.py -l mediumMaze -p SearchAgent -a fn=ucs
python pacman.py -l mediumDottedMaze -p StayEastSearchAgent
python pacman.py -l mediumScaryMaze -p StayWestSearchAgent
```

## A* Search
```
python pacman.py -l bigMaze -z .5 -p SearchAgent -a fn=astar,heuristic=manhattanHeuristic
```

## Finding the Four Corners in a Maze in the Shortest Path:
```
python pacman.py -l tinyCorners -p SearchAgent -a fn=bfs,prob=CornersProblem
python pacman.py -l mediumCorners -p SearchAgent -a fn=bfs,prob=CornersProblem
```

## Optimised Finding Four Corners in Shortest Path:
```
python pacman.py -l mediumCorners -p AStarCornersAgent -z 0.5
```

## Suboptimal, Greedy Pacman Search Algorithm
This one just searches for the closest dot to eat
```
python pacman.py -l trickySearch -p AStarFoodSearchAgent
```
