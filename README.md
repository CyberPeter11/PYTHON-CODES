print("hello world")
print("My is Name:Peter Uzoukwu")
print("Age: 25")
print("City: Lagos")
print("welcome to my world and, I really love you ")
print("my_number is = 07041543306")
user_name = input("What is your name? ")
print("Nice to meet you. " + user_name + "!")
if True:
    print("This line is indented!")
my_integer = 100
my_float = 20.7
my_string = "Welcome to my world"
is_learning = True
print("Value:", 100, " | Type:", type(my_integer))
print("Value:", 20.7, " | Type:", type(my_float))
print("Value:", "welcome to my world| Type:", type(my_string))
print("Value:", "T/F", " | Type:", type(is_learning))
num1 = 39
num2 = 5
addition = num1 + num2
subtraction = num1 - num2
multiplication = num1 * num2
division = num1 / num2
print(num1, "+", num2, "=", addition)
print(num1, "-", num2, "=", subtraction)
print(num1, "*", num2, "=", multiplication)
print(num1, "/", num2, "=", division)
print("\n-------------------------------------")
print("\n--- Asking for User Input ---")
user_name = input("What is your name? ")
print("Nice to meet you, " + user_name + "!")
print(" Student Marks")
math_score = int(input("Enter your Math score :"))
science_score = int(input("Enter your Science score: "))
total_score = math_score + science_score
print(f"Your total score is {total_score}!")

print("\n--- Day 4: Operators ---")

print("10 % 3 =", 10 % 3) 
print("Is 5 greater than 3?", 5 > 3)
print("Does 10 equal 10?", 10 == 10) 

print("\n Even/Odd Checker ")

number_to_check = int(input("Enter a whole number to check: "))

remainder = number_to_check % 2

if remainder == 0:
    print(f"The number {number_to_check} is EVEN!")
else:
    print(f"The number {number_to_check} is ODD!")
print(" Grade Calculator ")

score = int(input("Enter your test score (0-400): "))

if score >= 300:
    print("Grade: A - Amazing!")
elif score >= 200:
    print("Grade: B - Great job!")
elif score >= 100:
    print("Grade: C - You passed!")
else:
    print("Grade: F - Better luck next time.")



print("\n Number Patterns (For Loop)")
print("Here is a triangle made of numbers:")

for i in range(1, 7):
    print(str(i) * i)



print("\n ATM SIMULATION")

balance = 50000
pin = "1234"    

entered_pin = input("Welcome to Peter Uzoukwu Bank. Please enter your 4-digit PIN: ")

while entered_pin != pin:
    print("Incorrect PIN.")
    entered_pin = input("Try again: ")

print("\nLogin Successful!")


while True:
    print("\nMain Menu:")
    print("1. Check Balance")
    print("2. Deposit Money")
    print("3. Withdraw Money")
    print("4. Exit")
    
    choice = input("Select an option (1-4): ")
    
   
    if choice == "1":
        print(f"Your current balance is: ${balance}")
        
    elif choice == "2":
        amount = int(input("How much would you like to deposit? $"))
        balance = balance + amount
        print(f"Deposited ${amount}. New balance is: ${balance}")
        
    elif choice == "3":
        amount = int(input("How much would you like to withdraw? $"))
        
       
        if amount > balance:
            print("Insufficient funds! You don't have that much money.")
        else:
            balance = balance - amount
            print(f"Withdrew ${amount}. New balance is: ${balance}")
            
    elif choice == "4":
        print("Thank you for using Peter Uzoukwu Bank. Goodbye!")
        break  
        
    else:
        print("Invalid choice. Please select 1, 2, 3, or 4.")
print(" Day 8: Palindrome Checker ")
print("A palindrome is a word spelled the same forwards and backwards (like 'racecar').")

word = input("Enter a word to check: ")


word = word.upper() 


reversed_word = word[::-1] 

if word == reversed_word:
    print(f"Yes! '{word}' is a palindrome!")
else:
    print(f"No, '{word}' backwards is '{reversed_word}'.")



print("\n Day 9: To-Do List App ")


todo_list = []

while True:
    print("\nMenu:")
    print("1. Add a task")
    print("2. View all tasks")
    print("3. Exit app")
    
    choice = input("Choose an option (1-3): ")
    
    if choice == "1":
        new_task = input("What do you need to do? ")
        todo_list.append(new_task)  
        print(f"'{new_task}' has been added to your list!")
        
    elif choice == "2":
        print("\n--- Your Tasks ---")
        
        if len(todo_list) == 0:
            print("Your list is empty! You have nothing to do.")
        else:
            
            for task in todo_list:
                print("- " + task)
                
    elif choice == "3":
        print("Closing To-Do List App. Goodbye!")
        break 
        
    else:
        print("Invalid choice. Please type 1, 2, or 3.")
print(" Remove Duplicates (Using Sets) ")
messy_list = [1, 2, 2, 3, 4, 4, 4, 5, 5, 7]
print(f"Original messy list: {messy_list}")
clean_set = set(messy_list)
clean_list = list(clean_set)
print(f"Cleaned up list: {clean_list}")



print("\n Phone Book ")

#
phone_book = {
    "Alex": "555-1234",
    "Peter": "0704-154-3306",
    "John": "0905-059-5698"
}


print(f"Peter's phone number is: {phone_book['Peter']}")


phone_book["Sarah"] = "555-9999"
print(f"Updated Phone Book: {phone_book}")

phone_book["John"] = "09050595698"
print(f"Updated Phone Book: {phone_book}")

print("\n Function Calculator ")


def add_numbers(num1, num2):
    answer = num1 + num2
    return answer 

def multiply_numbers(num1, num2):
    return num1 * num2

def divid_numbers(num1, num2):
    return num1 / num2
    
sum_result = add_numbers(10, 5)
mult_result = multiply_numbers(10, 5)
div_result = divid_numbers(10, 5)

print(f"Using the add function (10 + 5): {sum_result}")
print(f"Using the multiply function (10 * 5): {mult_result}")
print(f"using the division function (10 / 5): {div_result}")# PYTHON-CODES
