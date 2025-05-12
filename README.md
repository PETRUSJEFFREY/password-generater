Java Program Documentation: Password Generator
This Java program demonstrates a simple and efficient way to generate a secure random password using a combination of uppercase letters, lowercase letters, special characters, and numbers. The main class, Tester, contains a main method and a static helper method named generatePassword.

The generatePassword method takes an integer parameter length, which determines the length of the password to be generated. It uses the Random class from the java.util package to randomly select characters.

To ensure the password meets basic security standards, the program includes at least one character from each of the following categories:

Lowercase letters: "abcdefghijklmnopqrstuvwxyz"

Uppercase letters: "ABCDEFGHIJKLMNOPQRSTUVWXYZ"

Special characters: "!@#$"

Numbers: "1234567890"

These characters are concatenated into a combinedChars string, from which the remaining characters of the password are randomly chosen. The first four characters of the password are explicitly set to include one from each of the four categories mentioned above, ensuring the password has a balanced composition. The rest of the password is filled by randomly picking characters from combinedChars.

The password is stored in a char[] array, which is a good practice in Java for handling sensitive data like passwords because it can be overwritten after use, unlike String objects that are immutable and stored in the string pool.

In the main method, the program calls generatePassword(8), which creates an 8-character password and prints it to the console.

This implementation is ideal for applications where basic password generation is needed without external libraries. It balances simplicity and functionality while ensuring the inclusion of different character types, improving the strength and unpredictability of the generated password.
