Guidelines for VHDL Coding
=====


Introduction
------------
This is a collection of rules and guidelines created by me (Jacob Watts) to help me write better and more consistant VHDL code.  I have found that when I write code that follows these guidelines, I am able to write code faster and with fewer errors.  I hope that you find these guidelines useful as well. This document is a work in progress and will be updated as I find new things to add. If you have any suggestions, please let me know.


Code Readability
----------------
The first rule of VHDL coding is to make your code readable. Code readability benefits not only yourself but also anyone else who may need to read your code.

* Use parenthese to control precedence in expressions.

* Avoid very long source code lines; 72 characters is a traditional limit. 

* Use indentation to highlight code structure. Two(2) spaces is enough to serve the purpose and will not use up too much of the line width. 


Names
-----

* Use a consistent case for each identifier. Use (clk, rst for clock and reset respectively)

* Use lower-case letters for signal names, variable names, and port names.

* Use upper-case letters for constants and user-defined types.

* Use underscore to make identifiers more readable: **low_byte** is better than **lowbyte**.

* Use meaningful and descriptive names when possible, but avoid names that are too long.


Suffix
------

* Use suffixes to indicate types of signals, variables, and constants.

* Use **_i** input signal, **_o** output signal, **_s** default signal.

* Use **_TB** for all testbench files.

* Use **_const** for all constrants files.

Common Signal Names 
-------------------

.. list-table:: Common VHDL Signal
   :widths: 25 25 50
   :header-rows: 1

   * - VHDL
     - Name
     - Heading row 1, column 3
   * - addr
     - address
     - Row 1, column 3
   * - Row 2, column 1
     - Row 2, column 2
     - Row 2, column 3

+------------------------+------------+----------+----------+
| Header row, column 1   | Header 2   | Header 3 | Header 4 |
| (header rows optional) |            |          |          |
+========================+============+==========+==========+
| body row 1, column 1   | column 2   | column 3 | column 4 |
+------------------------+------------+----------+----------+
| body row 2             | Cells may span columns.          |
+------------------------+------------+---------------------+
| body row 3             | Cells may  | - Table cells       |
+------------------------+ span rows. | - contain           |
| body row 4             |            | - body elements.    |
+------------------------+------------+----------+----------+
| body row 5             | Cells may also be     |          |
|                        | empty: ``-->``        |          |
+------------------------+-----------------------+----------+

