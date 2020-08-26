>> ### Exercise 1-2 Credit Card number validator
>> Credit card numbers follow certain pattern. A credit card number must have between 13 and 16 digits. The number must start with the following:
>>
>> * 4 for Visa cards
>> * 5 for MasterCard cards
>> * 37 for American Express cards
>> * 6 for Discover cards
>>
>> In 1954 Hans Luhn of IBM proposed an algorithm for validating credit card numbers. The algorithm is useful to determine whether a card number is entered correctly or is scanned correctly by a scanner. Almost all credit card numbers are generated following this validity check, commonly known as the *Luhn check* or the *Mod 10 check*. It can be destribed as follows. (For illustration, consider the card number **4388576018402626**.)
>>
>> 1. Double every second digit from the right to left. IF doubling of a digit results in a two-digit number, add the two digits to get a single digit number.
![Example CC](images/week01/creditcard.png)
>> 2. Now add all single-digit numbers from Step 1. `4 + 4 + 8 + 2 + 3 + 1 + 7 + 8 = 37`
>> 3. Add all digits in the odd places from right to left in the card number. `6 + 6 + 0 + 8 + 0 + 7 + 8 + 3 = 38`
>> 4. Sum the results from Step 2 and Step 3. `37 + 38 = 75`
>> 5.  If the result from Step 4 is divisable by **10**, the card number is valid; otherwise, it is invalid. For example **4388576018402626** is invalid, but the number **4388576018410707** is valid.
>>
>> Write a program that prompts the user to enter a credit card number as a string. Display whether the number is valid. Design your program using the following methods:
>>
>> ```cpp
>> // Return true if the card number is valid
>> bool isValid(const std::string& cardNumber);
>>
>> // Get the result from Step 2
>> int sumOfDoubleEvenPlace(const std::string& cardNumber);
>>
>> // Return this number if it is a single digit, otherwise,
>> // return the sum of the two digits
>> int getDigit(int number);
>>
>> // Return sum of odd-place digits in the card number
>> int sumOfOddPlace(const std::string& cardNumber);
>>
>> // Return true if substr is the prefix for cardNumber
>> bool startsWith(const std::string& cardNumber, const std::string& substr);
>> ```
>>
>> Write a test program that prompts the user to enter the string and character and display if the character is found.
>>
>{: .exercise}