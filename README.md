# Python-Caesar-Cipher

## Objective

The objective of this project is to implement a Caesar cipher encryption and decryption algorithm in Python. The Caesar cipher is a simple encryption technique in which each letter in the plaintext is shifted a certain number of places down or up the alphabet.

### Skills Learned

- Understanding encryption algorithms.
- Manipulating strings in Python.
- Handling user input and error checking.
- Implementing modular functions for encryption and decryption.

### Tools Used

- Python programming language
- Text editor (Riplet)


## Steps

1. First, I defined a Python function named caesar that takes three parameters: message, key, and mode.
The function is responsible for performing Caesar cipher encryption or decryption based on the provided message, encryption/decryption key, and mode.
<img width="633" alt="image" src="https://github.com/ammaarahadjiet/Password-Manager-Hosted-In-Cloud/assets/115926640/52b37b8b-753f-4158-98e2-c78113b16e16">

2. Inside the caesar function, I initialized a string named LETTERS containing the uppercase letters of the English alphabet.
I also initialized an empty string named translated to store the encrypted or decrypted message.
The message input is converted to uppercase to ensure consistency.
The encryption/decryption key is adjusted using the modulo operator % to keep it within the range of letters (0 to 25).
Iterate Through Each Character in the Message:
Using a for loop, I iterated through each character (i) in the input message.
Calculate Index and Perform Encryption/Decryption:
For each character i, I found its index in the LETTERS string using the find() method.
Depending on the specified mode ('encrypt' or 'decrypt'), I shifted the index of the letter to the right or left by the encryption/decryption key.
If the adjusted index exceeds the length of LETTERS, I wrapped it around to the beginning of the alphabet. Similarly, if it becomes negative, I wrapped it around to the end of the alphabet.
Build Encrypted/Decrypted Message:
After adjusting the index of each character, I appended the corresponding letter from the LETTERS string to the translated string.
Return Translated Message and Test:
Finally, I returned the translated message from the caesar function.
I also tested the function by calling it with sample inputs ("CAT", 6, 'encrypt' and "IGZ", 6, 'decrypt') and printing the results to verify the encryption and decryption processes.
