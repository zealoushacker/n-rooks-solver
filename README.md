# n-rooks

The total number of ways of placing _n_ nonattacking rooks on an _n x n_ chess board is _n!_

This solution has some interesting implications in pure and applied combinatorics, group theory, number theory, and statistical analysis.

# Exercise: n-rooks solutions calculator

* Develop an n-rooks solutions calculator by implementing [backbone.js](http://backbonejs.org/ "backbone.js") and using [jasmine](http://pivotal.github.com/jasmine/ "jasmine") for testing your code
* Make sure to drive out your logic first by writing jasmine specs for your models
  * Your models should capture all the details of the problem
* Views should be implemented with [mustache](http://mustache.github.com/ "mustache") or with similar templating tool
* Should render an 8x8 chessboard (_n_ is 8 by default for this exercise)
  * Use the [unicode chess rook symbol](http://en.wikipedia.org/wiki/Chess_symbols_in_Unicode "unicode chess symbols") to render rooks (example: &#9814;)
  * Allow the user to pick the color of the rook
  * Render the chessboard with html and css (no images) 
* Should calculate and keep track of all solutions
  * Should allow the user to change a default calculation timeout of 30s
  * Should keep track of all solutions discovered before the timeout period
  * Should allow the user to view calculated solutions by using the arrow keys

## Extra Credit:
* Display the timer as your validator/solver calculates valid solutions
* Use your timer code that you wrote as a guideline to implement a faster algorithm
* After you implement a more optimal solution, allow the user to pick the different algorithm

## Extra-Extra Credit:
* Allow the user to destroy cells on the chessboard (make holes) by clicking on them - damaged chessboard problem
* Based on destroyed cells, write a polynomial-time [O(n^k)] algorithm, to find the maximum number of non-attacking rooks that may be placed on the board

## Super-Extra Credit:
* Give the user the ability to pick between queens and rooks (n-queens problem)
* Implement the non-attacking queens solver

## References
* http://www.ams.org/bookstore/pspdf/mbk-63-prev.pdf (page 265)
* http://mathworld.wolfram.com/RooksProblem.html
* http://en.wikipedia.org/wiki/Rook_polynomial
