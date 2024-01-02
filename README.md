My ATM Project in C#

ATM Functions
* Withdraw Money
* Deposit Money
* Check Balance

Bank Users 
 * First Name
 * Last Name
 * Card Number
 * PIN
 * Account Balance


This C# code is part of a simple ATM machine simulation. It starts by defining a list of `cardHolder` objects, each representing a bank account with a card number, pin, first name, last name, and balance. 

The `Main` method begins by initializing a list of `cardHolder` objects, `cardHolders`, and populating it with four card holders. Each card holder is created using the `cardHolder` constructor, which takes five arguments: card number, pin, first name, last name, and balance.

The program then prints a welcome message and prompts the user to enter their card number.

After the `Main` method, a `debitCardNum` string and a `currentUser` object of type `cardHolder` are declared. These will be used to store the user's input and the corresponding `cardHolder` object, respectively.

The program then enters an infinite loop, which will continue until a valid card number is entered. Inside the loop, the program attempts to read a line of input from the console, which is expected to be the user's card number. It then tries to find a `cardHolder` in the `cardHolders` list whose `cardNum` matches the entered card number using the `FirstOrDefault` method. If a match is found, the corresponding `cardHolder` object is assigned to `currentUser` and the loop is broken. If no match is found, an error message is printed and the loop continues.

If an exception occurs during this process (for example, if the user's input cannot be read), the program catches the exception and prints an error message, then continues with the next iteration of the loop.

After a valid card number has been entered, the program prompts the user to enter their pin. It then initializes a variable `userPin` to store this pin, and enters another infinite loop, presumably to validate the pin in a similar manner to the card number. However, the code for this part of the process is not shown in the provided excerpt.
