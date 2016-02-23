1.	What is the function that creates Regex objects? 
Answer: re.compile()
2.	Why are raw strings often used when creating Regex objects? 
Answer: so backslashes do not have to be escaped
3.	What does the search() method return? 
Answer: Match objects
4.	How do you get the actual strings that match the pattern from a Match object?
Answer: group() returns strings of the matched text

5.	In the regex created from r'(\d\d\d)-(\d\d\d-\d\d\d\d)', what does group 0 cover? Group 1? Group 2? 
Answer: Group 0 is the entire match, group 1 covers the ﬁrst set of parentheses, and group 2 covers the second set of parentheses

6.	Parentheses and periods have speciﬁc meanings in regular expression syntax. How would you specify that you want a regex to match actual parentheses and period characters? 
Answer: periods & parentheses can be escaped with a backslash: \., \(, and \).

7.	The findall() method returns a list of strings or a list of tuples of strings. What makes it return one or the other? 
Answer: regex has no groups then list of strings return if regex has groups then list of   tuples returned.

8.	What does the | character signify in regular expressions? 
Answer:  matching “either, or” between two groups

9.	What two things does the ? character signify in regular expressions? 
Answer: n “ match zero or one of the preceding group” or non-greedy matching

10.	What is the difference between the + and * characters in regular expressions? 
Answer: + matches one or more. * matches zero or more
11.	What is the difference between {3} and {3,5} in regular expressions? 
Answer: {3} matches exactly three instances of the preceding group.  {3,5} matches between three and ﬁve instances.
12.	What do the \d, \w, and \s shorthand character classes signify in regular expressions? 
Answer:
13.	What do the \D, \W, and \S shorthand character classes signify in regular expressions? 
Answer:
14.	How do you make a regular expression case-insensitive? 
Answer:
15.	What does the . character normally match? What does it match if re.DOTALL is passed as the second argument to re.compile()? 
Answer:
16.	What is the difference between .* and .*?? 
Answer:
17.	What is the character class syntax to match all numbers and lowercase letters? 
Answer:
18.	If numRegex = re.compile(r'\d+'), what will numRegex.sub('X', '12 drummers, 11 pipers, five rings, 3 hens') return? 
Answer:
19.	What does passing re.VERBOSE as the second argument to re.compile() allow you to do? 
Answer:
20.	How would you write a regex that matches a number with commas for every three digits? It must match the following: s '42' s '1,234' s '6,368,745' but not the following: s '12,34,567' (which has only two digits between the commas) s '1234' (which lacks commas)
Answer:
21.	How would you write a regex that matches the full name of someone whose last name is Nakamoto? You can assume that the ﬁrst name that comes before it will always be one word that begins with a capital letter. The regex must match the following: s 'Satoshi Nakamoto' s 'Alice Nakamoto' s 'Robo?op Nakamoto' but not the following: s 'satoshi Nakamoto' (where the ﬁrst name is not capitalized) s 'Mr. Nakamoto' (where the preceding word has a nonletter character) s 'Nakamoto' (which has no ﬁrst name) s 'Satoshi nakamoto' (where Nakamoto is not capitalized) 
Answer:
22.	How would you write a regex that matches a sentence where the ﬁrst word is either Alice, Bob, or Carol; the second word is either eats, pets, or throws; the third word is apples, cats, or baseballs; and the sentence ends with a period? This regex should be case-insensitive. It must match the following: s 'Alice eats apples.' s 'Bob pets cats.' s 'Carol throws baseballs.' s 'Alice throws Apples.' s 'BOB EATS CATS.' but not the following: s 'Robo?op eats apples.' s 'ALICE THROWS FOOTBALLS.' s 'Carol eats 7 cats.'
Answer:
