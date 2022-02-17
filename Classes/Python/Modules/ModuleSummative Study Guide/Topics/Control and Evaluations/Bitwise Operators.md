# Bitwise Operators
- Bitwise operators work as if a number was represented by bits
- If you remember the counting game we did its the same as that
- Operators shuffle bits around to do what I like to call **magic math**, because reasons

## Operators
### x << y
- `<<` shifts all the number to the right y times
- same as multiplying x by 2^y
### x >> y
- `>>` Shifts all the ones and 0s to the right y times
- same as dividing x by 2^y

### x & y
- `&` is basically the `and` keyword
- if the same position in x and y is 1, that position is 1 in the output
### x | y
- `|` is basically the `or` keyword
- If there is a 1 in a given position of x or y, that position is 1 in the output
### ~x
- `~` flips all the bits
- 1s become 0s and 0s become 1s
### x ^ y
- `^` is basically exclusive or
- if one of the values in the same position of x and y is 1, that position is 1 in the output
- if both of the values in the same position of x and y is 1, that position is 0 in the output