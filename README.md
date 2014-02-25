edu-kata-render-table
=====================

Code kata to print a text table from input data.

## Problem

The `table.in` file contains empty-line separated groups. The first such group
are the column headers. Subsequent groups are the column data.

The `table.out` file contains the desired program output.

Write a program `table` that satisfies this shell command:

	$ ./table < table.in | diff - table.out

This command should generate no output, meaning the output of the program is
identical to `table.out`.

## Extra Credit

Can you separate the input, processing, and output phases of the program, so
that there are clean boundaries between them?

Do something reasonable for not-nice inputs:
* Empty input.
* Extra blank lines in arbitrary places.
* Missing elements from rows.
* Extra elements in rows.

Things you can do:
* Print appropriate messages to stderr.
* Try to render the table as best you can.