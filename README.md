# SEGT
*Spatial Evolutionary Game Theory*

This repo is used for implementing the Virual evolutionary game.

Game settings: there are two types of cells, namely defectors and cooperators. Their gains in the enviornment is according to this paroff matrix:

* When b > 1, the defectors will take up the main portion of the population eventually;
* When b < 1, then cooperators will take up the main portion.

| Cell type  | Cooperator (C)  | Defector (D)|
| :---        |    :----:   |          ---: |
| Cooperator (C)   | 1    | 0   |
| Defector (D) | b      | 0     |


We add another principle: each cell will become the type of its neighbor (8 neightbors in total) who has the highest payoff. Therefore, the type of a cell in each iteration is determined by not only its neighbors, but also the neighbors of its neighbors.

Another thing to be noticed is that, in the current implementation of the game (using JavaScript), we *did not* use mirroring in the boundary conditions.

Third-party tools:

[D3js Official site](https://d3js.org/)

[D3js official Wiki](https://github.com/d3/d3/wiki)

[P5js official site](https://p5js.org/)

[P5js Github Wiki](https://github.com/processing/p5.js/wiki)
