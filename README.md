This is an implementation of an interpreter for the Monkey language used by Thorsten Ball in his book "Writing an Interpreter in Go".  This is an educational exercise for me, and I'll be porting this interpreter to several other languages along the way to solidify and reinforce my understanding of the material.  The implementation will hew most closely to the language of the book itself, and over time I will go back through the authors full source code and port back in all of the features he leaves out in the book for the sake of focus and space.

### Some Differences from the Core Implementation
There are a few places where I have made changes to bring in language features I particularly like and wanted to understand more about how to implement them using the Pratt parser that the author implements.  They are listed below.

- Representation of integers:  you may use underscores in large numbers to break up the digits into more useful chunks (a la ```1_000_000```).  This was a feature from Ruby that I sorely miss in other languages when working with large numbers in code or in a REPL.
