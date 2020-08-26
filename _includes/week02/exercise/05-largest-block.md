>> ### Exercise 2-5 Largest block
>>
>> Given a square matrix with elements **0** or **1**, write a program that find a maximum square submatrix whose elements are all **1**`s. Your program should prompt the user to enter the number of rows in the matrix and then the matrix and displays the location of the first element in the maximum square submatrix and the number of the rows in the submatrix. Assume the maximum number of rows is **100**. 
>>
>> Here is a sample run:
>>
>>```output
>> Enter the number of rows for the matrix: ~~5~~
>> Enter the matrix row by row: 
>> ~~1 0 1 0 1~~ 
>> ~~1 1 1 0 1~~ 
>> ~~1 0 1 1 1~~
>> ~~1 0 1 1 1~~ 
>> ~~1 0 1 1 1~~ 
>> The maximum square submatrix is at (2, 2) with size 3
>>```
>>
>> Your program should implement and use the following function to find the maximum square matrix:
>>
>>```cpp
>> std::vector<int> findLargestBlock(const std::vector<std::vector<int>>& m);
>>```
>>
>> The return value is a vector that consists of three values. The first values are the row and column indices for the first element in the submatrix and the third value is the number of rows in the submstrix.
>>
>{: .exercise}