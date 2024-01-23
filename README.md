### Approach
Connected to encrypted and unencrypted servers using imported socket functions
Use find method to solve wordle: given the marks, create a list of characters marked 1 or 2 (no repeats), eliminate the words that do not contain the characters
When word was found, print flag

### Challenges
There were previous guessing strategies that combed through each word and removed words without characters that were marked with 1 or 2
The first one had a mistake in combing through the list (skipping words) -> made a copy of the wordlist to comb through, removed words from another word list, and then recopied to comb through the words with the next character
The final iteration of the guessing strategy is similar to the second one, except it cuts down on the lines of code (more efficient)
Instead of checking for 0, 1, or 2, and then removing words from the list that way, I checked for any characters that was on the character list (list of characters that were marked 1 or 2)

### Testing
Tested load_words() using the print function
Tested guess_word() using temporary word list and previous guess result
Changed word list and guess result to thoroughly test
Tested connect_server() and connect_encrypted_server() through print functions and checked for responses
Tested client and client.py by running through terminal with all availble options
