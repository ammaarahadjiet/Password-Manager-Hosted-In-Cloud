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

2. Inside the caesar function, I initialized a string named LETTERS containing the uppercase letters of the English alphabet. I also initialized an empty string named translated to store the encrypted or decrypted message. The message input is converted to uppercase to ensure consistency. The encryption/decryption key is adjusted using the modulo operator % to keep it within the range of letters (0 to 25).
<img width="626" alt="image" src="https://github.com/ammaarahadjiet/Password-Manager-Hosted-In-Cloud/assets/115926640/1c213f7e-4999-4c35-912c-44e9930c0256">

3. Using a for loop, I iterated through each character (i) in the input message.
<img width="631" alt="image" src="https://github.com/ammaarahadjiet/Password-Manager-Hosted-In-Cloud/assets/115926640/25adad23-11ea-46d9-847d-b204be814476">


4. For each character i, I found its index in the LETTERS string using the find() method. Depending on the specified mode ('encrypt' or 'decrypt'), I shifted the index of the letter to the right or left by the encryption/decryption key. If the adjusted index exceeds the length of LETTERS, I wrapped it around to the beginning of the alphabet. Similarly, if it becomes negative, I wrapped it around to the end of the alphabet.
<img width="631" alt="image" src="https://github.com/ammaarahadjiet/Password-Manager-Hosted-In-Cloud/assets/115926640/b431b81b-a35a-4a20-9710-148efc63d7e9">


5. After adjusting the index of each character, I appended the corresponding letter from the LETTERS string to the translated string.
<img width="633" alt="image" src="https://github.com/ammaarahadjiet/Password-Manager-Hosted-In-Cloud/assets/115926640/6033068b-9591-4866-bf0a-e96a1a65ed35">

6. Finally, I returned the translated message from the caesar function. I also tested the function by calling it with sample inputs ("CAT", 6, 'encrypt' and "IGZ", 6, 'decrypt') and printing the results to verify the encryption and decryption processes.
<img width="630" alt="image" src="https://github.com/ammaarahadjiet/Password-Manager-Hosted-In-Cloud/assets/115926640/3114b5eb-93d0-466f-bd29-0e516b6ed650">
<img width="517" alt="image" src="https://github.com/ammaarahadjiet/Password-Manager-Hosted-In-Cloud/assets/115926640/bff7bfc2-3a8b-4557-9a46-8a918ab508d9">

