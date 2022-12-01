Guidelines for VHDL Coding
=====


Introduction
------------
This is a collection of rules and guidelines created by me (Jacbo Watts) to help me write better and more consistant VHDL code.  I have found that when I write code that follows these guidelines, I am able to write code faster and with fewer errors.  I hope that you find these guidelines useful as well. This document is a work in progress and will be updated as I find new things to add. If you have any suggestions, please let me know.


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
