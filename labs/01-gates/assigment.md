1. Equations of all three versions of logic function f(c,b,a): nope

   ![Logic function](images/equations.png)![image](https://user-images.githubusercontent.com/99815316/155214467-4f764439-c602-4acd-b820-bde35af895c7.png)


2. Listing of VHDL architecture from design file (`design.vhd`) for all three functions. Always use syntax highlighting, meaningful comments, and follow VHDL guidelines:

```vhdl
architecture dataflow of demorgan is
begin
    f_o      <= (not(b_i) and a_i) or (not(c_i) and not(b_i)); -- WRITE YOUR CODE HERE
    f_nand_o <= (((b_i nand b_i) nand a_i) nand ((b_i nand b_i) nand (c_i nand c_i))); -- WRITE YOUR CODE HERE
    f_nor_o  <= (((a_i nor a_i) nor b_i) nor (b_i nor c_i)) nor (((a_i nor a_i) nor b_i) nor (b_i nor c_i))-- WRITE YOUR CODE HERE
end architecture dataflow;
```

3. Complete table with logic functions' values:

| **c** | **b** |**a** | **f(c,b,a)_ORG** | **f(c,b,a)_NAND** | **f(c,b,a)_NOR** |
| :-: | :-: | :-: | :-: | :-: | :-: |
| 0 | 0 | 0 | 1 |1  |1  |
| 0 | 0 | 1 | 1 | 1 | 1 |
| 0 | 1 | 0 | 0 | 0 | 0 |
| 0 | 1 | 1 | 0 | 0 | 0 |
| 1 | 0 | 0 | 0 | 0 | 0 |
| 1 | 0 | 1 | 1 | 1 | 1 |
| 1 | 1 | 0 | 0 |  0| 0 |
| 1 | 1 | 1 | 0 | 0 | 0 |

### Distributive laws

1. Screenshot with simulated time waveforms. Always display all inputs and outputs (display the inputs at the top of the image, the outputs below them) at the appropriate time scale!

   ![your figure]()![image](https://user-images.githubusercontent.com/99815316/155215175-ee205206-ec21-4e82-af72-3b2af9ff96e5.png)

2. Link to your public EDA Playground example:

   [https://www.edaplayground.com/...](https://www.edaplayground.com/...)
https://www.edaplayground.com/x/WsAC
