# Lab 2: YOUR_FIRSTNAME LASTNAME

### 2-bit comparator

1. Karnaugh maps for other two functions:

   Greater than:
![image](https://user-images.githubusercontent.com/99815316/156237379-1a60afb8-974c-44a3-8aac-00191913eb74.png)



   Less than:
   ![image](https://user-images.githubusercontent.com/99815316/156238043-8699c8f3-a730-4405-aeb2-7d1243843ef5.png)




2. Equations of simplified SoP (Sum of the Products) form of the "greater than" function and simplified PoS (Product of the Sums) form of the "less than" function.
![image](https://user-images.githubusercontent.com/99815316/156238079-d2870ebd-e3a7-45ef-a6ed-f33ab392e769.png)
![image](https://user-images.githubusercontent.com/99815316/156238120-5a93bafa-4f9c-4cc8-83ab-718d003b19b5.png)


   ![Logic functions](images/comparator_min.png)

### 4-bit comparator

1. Listing of VHDL stimulus process from testbench file (`testbench.vhd`) with at least one assert (use BCD codes of your student ID digits as input combinations). Always use syntax highlighting, meaningful comments, and follow VHDL guidelines:

   Last two digits of my student ID: **xxxx??**

```vhdl
    p_stimulus : process
    begin
        -- Report a note at the beginning of stimulus process
        report "Stimulus process started" severity note;

        -- First test case
        s_b <= "BCD_OF_YOUR_SECOND_LAST_ID_DIGIT"; -- Such as "0101" if ID = xxxx56
        s_a <= "BCD_OF_YOUR_LAST_ID_DIGIT";        -- Such as "0110" if ID = xxxx56
        wait for 100 ns;
        -- Expected output
        assert ((s_B_greater_A = 'WRITE_CORRECT_VALUE_HERE') and
                (s_B_equals_A  = 'WRITE_CORRECT_VALUE_HERE') and
                (s_B_less_A    = 'WRITE_CORRECT_VALUE_HERE'))
        -- If false, then report an error
        report "Input combination COMPLETE_THIS_TEXT FAILED" severity error;

        -- Report a note at the end of stimulus process
        report "Stimulus process finished" severity note;
        wait;
    end process p_stimulus;
```

2. Text console screenshot during your simulation, including reports.

![image](https://user-images.githubusercontent.com/99815316/156238181-17d62268-97db-4815-970d-8d0491624665.png)
![image](https://user-images.githubusercontent.com/99815316/156238205-1bd59f5e-8301-492f-a098-e692aa31d38e.png)

   ![your figure]()


3. Link to your public EDA Playground example:
4. https://www.edaplayground.com/x/7Wzu

   [https://www.edaplayground.com/...](https://www.edaplayground.com/...)
