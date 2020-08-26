>> ### Exercise 2-2 Find genes
>>
>> Biologists use a sequence of letters **A**, **C**, **T** and **G** to model a *genome*. A *gene* is a substring of a genome that starts after a triplet of **ATG** and ends before a triplet of **TAG**, **TTA** or **TGA**. Futhermore, the length of a gene string is a multiple of **3** and the gene does not contain any of the triplets **ATG**, **TAG**, **TTA** and **TGA**. 
>>
>> Write a program that prompts the user to enter a genome and displays all genes in the genome. If no gene is found in the input sequence, displays no gene.
>>
>> Here is the sample run:
>>
>>```output
>> Enter a genome string: ~~TTATGTTTTAAGGATGGGGCGTTAGTT~~
>> TTT
>> GGGCGT
>>```
>>
>{: .exercise}