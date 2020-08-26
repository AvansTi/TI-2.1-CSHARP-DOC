>> ### Exercise 1-3 Counting characters
>>
>> Write a method that counts the occurence of each letter in the string using the following header:
>>
>>```cpp
>> void count(const char s[], int counts[]);
>>```
>>
>> where `counts` is an array of ***26*** integers, `counts[0], counts[1], ...`, and `counts[25]` count the occurence of ***a,b,....*** and ***z***, respectively. Letters are not case-sensitive, i.e. letter ***A*** and ***a*** are counted the same as ***a***
>>
>> Write a test program that reds a string, invokes the `count` method, and displays the non-zero counts. Here is a sample run of the program:
>>
>> ```output
>> Enter a string: ~~Welcome to New York!~~
>> c: 1 times
>> e: 3 times
>> k: 1 times
>> l: 1 times
>> m: 1 times
>> n: 1 times
>> o: 3 times
>> r: 1 times
>> t: 1 times
>> w: 2 times
>> y: 1 times
>> ```
>>
>{: .exercise}