# Positional Cube Notation Calculator

A simple solution for computing complement of Boolean functions.
Given a Boolean function F as a PCN cube list returns F' (complemented function) also as a PCN cube list.

### Input File

#### Input File Rulles
Input files use a simple text file format. The file format uses the above skeleton:

1. First line of the file is a number (positive integer) declaring how many variables are in the equation. Variables numbering starts with index 1.
2. Second line of the file is a number (positive integer) declaring how many cubes are in this cube list.
3. Each of the subsequent lines of the file describes one cube, that means one line for every cude for all cubes defined at second line of the input file. Each line should follow the above format
  1. The first number on the line says how many variables are not don’t cares in this cube. 
  2. The next numbers use the next form. If this number of variables is, e.g., 5, then the next 5 numbers on the line specify the true or complemented form of each variable in this cube. A simple convention is used: if variable x_k appears in true form, then put integer "k" on the line else put integer "-k" on the line. The file will always order these variables in increasing index order.
  
#### Example of input file.
Suppose we have this function as input:

    F(x1,x2,x3,x4,x5,x6) =x2x4x5’ + x2’x4’x6 + x1x2x3’x4’ + x5x6

Then the input file format would look like this:

    6
    4
    3 2 4 -5
    3 -2 -4 6
    4 1 2 -3 -4
    2 5 6
 
