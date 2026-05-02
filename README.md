1.GUESS THE NUMBER:

import random



\# Generate a random number between 1 and 100

number = random.randint(1, 100)



print("Welcome to Guess the Number!")

print("I'm thinking of a number between 1 and 100.")



while True:

&#x20;   guess = int(input("Enter your guess: "))



&#x20;   if guess < number:

&#x20;       print("Too low! Try again.")

&#x20;   elif guess > number:

&#x20;       print("Too high! Try again.")

&#x20;   else:

&#x20;       print("🎉 Congratulations! You guessed the number!")

&#x20;       break





2\. Collatz Sequence Program

def collatz(n):

&#x20;   while n != 1:

&#x20;       print(n, end=" -> ")

&#x20;

&#x20;       if n % 2 == 0:

&#x20;           n = n // 2   # even number

&#x20;       else:

&#x20;           n = 3 \* n + 1   # odd number

&#x20;

&#x20;   print(1)



\# Take input from user

num = int(input("Enter a positive integer: "))



if num > 0:

&#x20;   collatz(num)

else:

&#x20;   print("Please enter a positive number.")



3.Adding Bullets to Wiki Markup:

import pyperclip

text = pyperclip.paste() #hi hello

text='\* '+text.replace('\\n','\\n\*')

pyperclip.copy(text)

print(text)



Text book:

import pyperclip

text = pyperclip.paste()

lines = text.split('\\n')

for i in range(len(lines)):

&#x20;   lines\[i] = '\* ' + lines\[i]

text = '\\n'.join(lines)

pyperclip.copy(text)

