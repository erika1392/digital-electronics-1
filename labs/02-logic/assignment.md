# Lab 2: YOUR_FIRSTNAME LASTNAME

### 2-bit comparator

1. Karnaugh maps for other two functions:

   Greater than:
![image](https://user-images.githubusercontent.com/99815316/156237379-1a60afb8-974c-44a3-8aac-00191913eb74.png)

   [image](https://user-images.githubusercontent.com/99815316/155343651-49c4ceb4-1e88-4555-a70f-4b5ae92fd5a7.png)


   Less than:
   ![image](https://user-images.githubusercontent.com/99815316/156237417-b1712d03-f7c5-4537-80b7-ba0364cf35a3.png)


   [image](https://user-images.githubusercontent.com/99815316/155343707-9a075af8-6df5-4f5d-98fa-b17a720edde4.png)


2. Equations of simplified SoP (Sum of the Products) form of the "greater than" function and simplified PoS (Product of the Sums) form of the "less than" function.
![image](https://user-images.githubusercontent.com/99815316/156237466-dbcf3c96-6546-480b-8ef3-172b1bc6addc.png)

   ![Logic functions](images/comparator_min.png)
![image](https://user-images.githubusercontent.com/99815316/156237527-0735a2a5-93e6-48eb-a4eb-87120ddb0f06.png)

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
![image](https://user-images.githubusercontent.com/99815316/156237604-8951e1ff-97d4-4160-887c-205715f22302.png)

   ![your figure]()
   ![image](https://user-images.githubusercontent.com/99815316/156237643-b298efb9-ab93-4326-8ab8-97d43b9eeea4.png)


3. Link to your public EDA Playground example:
4. https://www.edaplayground.com/x/7Wzu

   [https://www.edaplayground.com/...](https://www.edaplayground.com/...)
