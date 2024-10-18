File Globbing is used to fill in the paths/ name of the files instead dof manually typing it out.
There are operators used for "expansions" which match with the corresponding names of the files/directories.

## Methods

  1. '*' is used to replace the argument with a matching pattern. If zero files are matched, then it will remain unchanged.
     The '*' matches any character except the '/' or a leading '.'.

  2.  '?' matches for a single character instead of the corresponding whole file name.
  3.  If there are multiple potential characters to be matched then they can be placed inside '[]' to check for the characters inside the paranthesis.
    The globbing is done on the basis of file paths.

  4. The converse can be done too. Files which do not want to be matched can be placed within the [] and adding a invert(!) to exclude the particular file names.
