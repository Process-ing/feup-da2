## Objectives of the Project

The main objective of this project is to develop a tool that can solve the TSP on undirected graphs, using:

- a backtracking approach, with branch-and-bound;
- a 2-approximation algorithm for complete graphs that respect the triangular inequality;
- another heuristic that either gives better results for the same class of graphs or has a lower time complexity, while providing similar results;
- a heuristic that works well for any undirected graph, even if incomplete or not respecting the triangular inequality.

## Instructions to Run

1. Clone the repository
2. Run the following commands on the terminal:
    ```
    cd feup-da2                    # Open project
    mkdir build && cd build        # Create and open build directory
    cmake .. && cmake --build .    # Build project
    ./feup-da2                     # Run project
    ```

If the project is being run in the CLion terminal, make sure the option "Emulate terminal in output console" is enabled
in the Run/Debug configurations. This is necessary for capturing inputs for our program.

## Using Custom Datasets

Custom Datasets can be used in the project. To use them follow these instructions:
1. Put the files in a folder named "graph/Custom/" in the main project directory according to the following rules:
    - The **Nodes** file should be named "nodes.csv"
    - The **Edges** file should be named "edges.csv"
    - The overall structure of the CSV files should be the same as the ones in the fully connected or real-world datasets
2. When starting the program, select the option ```[4]``` in the menu to load a custom dataset

The structure should be like:
```
$ tree graph

  graph
    ├── Custom
    │      ├── edges.csv
    │      └── nodes.csv
    ├── Extra Fully Connected
    ├── Real World
    └── Toy
```

## Tips and Tricks (for anyone doing a similar project)

- Try to think about the algorithms before starting to develop the code. This will give a clearer understanding of what you will and will not need and define a structure that better suits the project.
- You can learn a lot about the TSP and its algorithms and heuristics by searching online.

## Contributors and Results

- [Bruno Oliveira](https://github.com/Process-ing)
- [Rodrigo Coelho](https://github.com/racoelhosilva)
- [Vítor Pires](https://github.com/vitormpp)

Final Grade: 20.0/20
