# sample-python-program
Excercise from learnpython.org
In this exercise, you will need to print an alphabetically sorted list of all functions in the re module, which contain the word find.


# Source code:

import re

find_members = []
for member in dir(re):
    if "find" in member:
        find_members.append(member)

print(sorted(find_members))
