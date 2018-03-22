# Guess.Py
Guessing Game


 #This is a guess the number game.
 
 import random
 
  guessesTaken = 0
 
 print('Bonjour! What shall I call you?')
  myName = input()
 
  number = random.randint(1, 33)
 print('Great, ' + myName + ', I have a number between 1 and 33 in my head.')

 while guessesTaken < 10:
     print('Take a wild guess.') 
     guess = input()
     guess = int(guess)

     guessesTaken = guessesTaken + 1

     if guess < number:
         print('A little higher than that!') 

     if guess > number:
         print('A littler lower than that!')

     if guess == number:
         break

 if guess == number:
     guessesTaken = str(guessesTaken)
     print('Awesome, ' + myName + '! You guessed the right number in ' + guessesTaken + ' tries!')

 if guess != number:
     number = str(number)
     print('Sorry. The number I was thinking of was ' + number)
