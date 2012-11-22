# n-rooks

The total number of ways of placing _n_ nonattacking rooks on an _n x n_ chess board is _n!_

This solution has some interesting implications in pure and applied combinatorics, group theory, number theory, and statistical analysis.

# Exercise: n-rooks validator

* Develop an n-rooks validator by implementing [backbone.js](http://backbonejs.org/ "backbone.js") and using [jasmine](http://pivotal.github.com/jasmine/ "jasmine") for testing your code
* Should allow the user to specify the size of the chessboard (_n_)
  * Should validate that _n_ is at least 2
  * For extra credit, allow the user to start with an _m x n_ chess board (different number of rows and columns)
* Should render the board based on the value of _n_ (or _m_ and _n_ when attempting for extra credit)
  * Use the [unicode chess rook symbol](http://en.wikipedia.org/wiki/Chess_symbols_in_Unicode "unicode chess symbols") to render rooks (example: &#9814;)
  * Allow the user to pick the color of the rook
  * Render the chessboard with html and css (no images) 
* Should calculate and keep track of all solutions after the user specifies the size of the board
  * Should allow the user to change a default calculation timeout of 30s
  * Should keep track of all solutions discovered before the timeout period
  * Note: This should prevent long runs for large values of _n_ (or _m_ and _n_ in the extra credit case)
* Should allow the user to enter solutions by placing rooks onto the board
* Should validate user entered solutions by verifying the following conditions:
  * an _n x n_ chessboard may have no more than _n_ non-attacking rooks
  * For extra credit, figure out what the maximum number of non-attacking rooks may be placed on an _m x n_ board and validate user entry


## References
* http://mathworld.wolfram.com/RooksProblem.html
* http://en.wikipedia.org/wiki/Rook_polynomial
