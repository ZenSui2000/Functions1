# Functions1
1.subject_marks = [('Sachin Tendulkar', 34357), ('Ricky Ponting', 27483), ('Jack Kallis', 25534), ('Virat Kohli', 24936)]
print("Original list of tuples:")
print(subject_marks)
subject_marks.sort(key = lambda x: x[1])
print("\nSorting the List of Tuples:")
print(subject_marks)

2.numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

squared_numbers = list(map(lambda x: x**2, numbers))

print("Squared numbers:", squared_numbers)

3.numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

string_tuple = tuple(map(lambda x: str(x), numbers))

print(string_tuple)

4.from functools import reduce

numbers = list(range(1, 26))

product = reduce(lambda x, y: x * y, numbers)

print("Product:", product)

5.def divisible_by_2_and_3(num):
    return num % 2 == 0 and num % 3 == 0

def main():
    
    numbers = [2, 3, 6, 9, 27, 60, 90, 120, 55, 46]
    
    filtered_numbers = list(filter(divisible_by_2_and_3, numbers))

    print("Filtered Numbers:", filtered_numbers)

if __name__ == '__main__':
    main()
    
    6. def is_palindrome(string):
    
    string = string.replace(" ", "").lower()
    
    return string == string[::-1]

strings = ['python', 'php', 'aba', 'radar', 'level']

palindromes = list(filter(lambda x: is_palindrome(x), strings))

print("Palindromes in the list:")
for palindrome in palindromes:
   
    print(palindrome)
