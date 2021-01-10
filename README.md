#DISREGARD BELOW
print("""
Welcome to SheHacks V
Python Challenge for Team - 16
This is the number guessing game, may the odds be ever in your favour!
""")

player_name = input("Hello, what's your name? ")

print("Okay " + player_name + "!")

import random

input_var1 = input("What is your favorite month? ")
input_var2 = input("What is your favorite year? ")


value = random.randint(int(input_var1),int(input_var2))

guess = int(input("Now guess a number! "))


while value != "guess":

  print

  if guess < value:

    print ("Incorrect. The number is higher")

    guess = int(input("Now guess a number!"))

  elif guess > value:

    print ("Incorrect. The number is lower")

    guess = int(input("Now guess a number! "))

  else:

    print ("Congratulations! You guessed the number")

    break
