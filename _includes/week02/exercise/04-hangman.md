>> ### Exercise 2-4 Hangman
>>
>> Write a hangman games that randomly generates a word and prompts the user to guess one letter at a time, as shown in the sample run.
>> Each letter in the word is displayed in an asterik. When the user makes a correct guess, the actual letter is then displayed. When the user finishes a word, display the number of misses and ask the user whether to continue for another word. Declare an array to store the words as follows:
>>
>>```cpp
>> std::vector<std::string> words = {"write", "that", "school, ...};
>>```
>>
>>```output
>> (Guess) Enter a letter in the word ******* > ~~p~~
>> (Guess) Enter a letter in the word p****** > ~~r~~ 
>> (Guess) Enter a letter in the word pr**r** > ~~p~~
>>      p is already in the word
>> (Guess) Enter a letter in the word pr**r** > ~~o~~
>> (Guess) Enter a letter in the word pro*r** > ~~g~~
>> (Guess) Enter a letter in the word progr** > ~~n~~
>>      n is not in the word
>> (Guess) Enter a letter in the word progr** > ~~m~~
>> (Guess) Enter a letter in the word progr*m > ~~a~~
>> The word is program. You missed 1 time.
>>
>> Do you want to guess for another word? enter y or n >
>>```
>>
>{: .exercise}