OPL Goodies
============

[OPL](http://www-01.ibm.com/software/commerce/optimization/modeling/index.html) is the modeling language used in CPLEX. It's the most powerful mathematical & constraint programming language that I know of. If you ended up here, you're probably an OPL believer yourself!

* opl_json.js
    * Provides a javascript implementation to export objects in OPL to JSON
* opl_print.js
    * Provides (s)printf functions using Java interfacing
* opl_popups.js
    * Provides window alerts & confirmations using Java interfacing
* sudoku.mod
    * A CP model to solve sudoku grids
* sudoku_samurai.mod
    * A CP model to solve samurai sudoku grids


--
OPL only has very basic javascript functionality
e.g. 
- typeof checks can't have type coercion,
- there's no RegExp, no array.push, ...

Hence these tools :)

--
Example:

    dvar int x[R];
    // ..
    execute {
      includeScript("jsonopl.js");
      writeln(stringify(x));
    }
