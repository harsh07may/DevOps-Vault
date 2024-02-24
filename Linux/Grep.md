
**Global Regular Expression Print** or grep is a powerful command-line utility in Linux/Unix systems used for searching text within files.
`grep` searches for patterns you specify and prints out any lines in a file that contain the matching pattern.
![[Pasted image 20240224204716.png]]


﻿
```bash
# Search for a pattern in a file and print all matching lines
grep [pattern] <filename>

# Print all lines that do not match the pattern
grep -v [pattern] <filename>

# Print the lines that contain the numbers 0 through 9
grep [0-9] <filename>

# Print context of lines (specified number of lines above and below the pattern) 
# for matching the pattern. Here, the number of lines is specified as 3
grep C 3 [pattern] <filename>
```
