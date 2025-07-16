'''Task 1'''
people = [
    {"name": "Gaya", "age": 25},
    {"name": "Kathir", "age": 17},
    {"name": "Sanya", "age": 58},
    {"name": "Dyuthi", "age": 16}]
adults = list(map(lambda person: person, filter(lambda person: person['age'] >= 18, people)))
print(adults)

''''Task 2'''
from functools import reduce
numbers = [2, 3, 4, 5]
product = reduce(lambda x, y: x * y, numbers)
print("The product of all numbers in the list is:", product)

''''Task 3'''
numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
squares_of_evens = list(map(lambda x: x**2, filter(lambda x: x % 2 == 0, numbers)))
print(squares_of_evens)

'''''Task 4'''
string_to_int = lambda s: int(s)
print(string_to_int("10"))

'''Task 5'''
import datetime
now = datetime.datetime.now ()
year= lambda x: x.year
month = lambda x: x.month
day = lambda x: x.day
print ( year ( now ) )
print ( month ( now ) )
print ( day ( now ) )

'''Task 6'''
n = 10
fibonacci = lambda n: reduce(lambda x, _: x + [x[-1] + x[-2]], range(n - 2), [0, 1])
print(fibonacci(n))
