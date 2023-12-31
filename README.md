# Checkpoint-Recursion

## palindrome_checker Algorithm:

This is the main algorithm that interacts with the user by prompting the user to input a word and then calls the palindrome function to check if the input word is a palindrome.

## palindrome Function:

This is a recursive function that checks if a given word is a palindrome. It takes a single argument, word, which is the string to be checked.

> > The function uses the following logic:

> > > If the length of the word is less than 2 characters (i.e., it's a single character or an empty space), it immediately returns "word is a palindrome" as the base case. A single character or an empty space is considered a palindrome.

> > > If the first character of the word is not the same as the last character, it returns "word is not a palindrome" because a non-matching first and last character indicates it's not a palindrome.

> > > If neither of the above cases is met, the function recursively calls itself after removing the first and last characters from the word. It continues to call itself with the trimmed word until one of the base cases is met.

> > > The function then returns the result.

> ### Variable Declarations:

> > tag and trimmed are initialized as empty strings.  
> > i is an integer counter, and  
> > n is assigned the length of the input word.

## Base Case = 1:

### If the length of the input word is less than 2 or if the word is an empty space (a single character or an empty string), the function returns "word is a palindrome." This is the base case that stops the recursion.

### Else If:

> > If the first and last characters of the input word (at indices 0 and n - 1) do not match, it means the word is not a palindrome. The function returns "word is not a palindrome."

### Else (Recursive Case):

> > > If the base cases are not met, the function enters loop block
> > > A FOR loop is used to create a new string called trimmed, which is the original word with the first and last characters removed.

> > > The palindrome function is called recursively with the trimmed word, and the result is stored in the tag variable.

### Return Tag:

> > > The function returns the value of tag, which will be either "word is a palindrome" or "word is not a palindrome" based on the input.

# In summary

The **palindrome_checker** algorithm collects a word from the user and uses the **palindrome** function to determine if it's a palindrome. The **palindrome** function employs recursion and base cases to make this determination. The result is then displayed to the user.
