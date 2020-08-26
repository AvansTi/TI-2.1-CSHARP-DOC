>> ### Exercise 3-3 Intersection
>>
>> Write a function that returns the intersection of two vectors using the following header:
>>
>> ```cpp
>> template<typename T>
>> std::vector<T> intersect(const std::vector<T>& v1, const std::vector<T>& v2);
>> ```
>>
>> The intersection of two vectors contains the common elements that appear in both vectors. For example, the intersection of two vectors {2, 3, 1, 5} and {3, 4, 5} is {3, 5}. Write a test program that prompts the user to enter two vectors, each with five strings, and displays their intersection. Here is a sample run:
>>
>>```output
>> Enter five strings for vector1:
>> ~~Atlana Dallas Chicago Boston Denver~~
>> Enter five strings for vector2:
>> ~~Dallas Tampa Miami Boston Richmond~~
>> The common strings are Dallas Boston
>>```
>>
>{: .exercise}