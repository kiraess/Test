# Test
number guessing practice

low = 0
high = 100

print("Please think of a number between 0 and 100")
while True:
    guess = (low + high)/2
    guess = int(guess)
    print("is your secret number " + str(guess) + "?" )
    id = input("Enter 'h' to indicate the guess is too high. Enter 'l' to "
           "indicate the guess is too low. Enter 'c' to indicate I guessed "
           "correctly.")
    if id == 'h':
        high = guess
    elif id == 'l':
        low = guess
    elif id == 'c':
        break
    else:
        print("Sorry, I did not understand your input.")
print ("Game over. You secret number was: " + str(guess))


