
I have used jupyter notebook to compile this code.
Question 1:

This code defines a function called "sentence_check" that takes in two sentences and a list of synonyms represented as tuples. The function converts the sentences to lowercase and splits them into lists of words. It then checks if the number of words in the two sentences are not equal, in which case it returns False. If the number of words is equal, it iterates through the synonyms and replaces the words in the sentences with their synonyms. Finally, it checks if the modified sentences are equal and returns True if they are, otherwise False. Two test cases are provided at the end of the code to demonstrate how the function can be used.

Question 2:

This code is a function that takes in two sentences (sentence1 and sentence2) and a list of synonyms (synonyms) and checks if the two sentences are equivalent. The function first converts the sentences to lowercase and splits them into a list of words. It then checks if the number of words in the two sentences are not equal, and if so, returns False.

The function then creates a dictionary (synonyms_dict) to store the synonyms and their corresponding synonyms. This is done by iterating through the list of synonyms and adding each word and its corresponding synonym to the dictionary. For example, if the synonyms list contains the tuple ("eat", "consume"), the dictionary would contain the key "eat" with the value ["consume"] and the key "consume" with the value ["eat"].

The function then defines a nested function called dfs (short for depth first search) that takes in a word, a target word, and a list of visited words. The function checks if the current word is the target word and if so, returns True. If the word has already been visited, it returns False. If the word is in the synonyms dictionary, the function iterates through its corresponding synonyms and performs the dfs function on each one. If none of these conditions are met, the function returns False.

The main function then uses the zip function to iterate through the words in the two sentences and performs the dfs function on each pair of words. If the dfs function returns False for any pair of words, the main function returns False. If the dfs function returns True for all pairs of words, the main function returns True. The code then includes test cases to demonstrate the function's usage.


