# PRODIGY_CS_01

Welcome to PRODIGY_CS_01! This is a project that aims to allow users to input a message and a shift value to perform encryption and decryption.

## Function

The caesar cipher encryption function works on the following:
1. Takes 'text' and 'shift' as inputs.
2. Iterates through each character in the text.
3. If the character is a letter, it calculates the shifted position and converts it back to a character.
4. If the character is not a letter, it remains unchanged.
5. Returns the encrypted text.

The decrpyt function works similar to the encrypt function but subtracts the shift amount to reverse the encryption.

## Usage

1. Encrypts the plaintext "PRODIGY INFOTECH" with a shift of 4 to "tvshmkc mrjsxigl".
   '''
   def encrypt(plaintext, key):
    ciphertext = ''
    for letter in plaintext:
        letter = letter.lower()
        if letter != ' ':
            index = letters.find(letter)
            if index == -1:
                ciphertext += letter
            else:
                new_index = (index + key) % num_letters
                ciphertext += letters[new_index]
        else:
            ciphertext += ' '
    return ciphertext
   '''
3. Decrypts the encrypted text back to the original plaintext "prodigy infotech".
   '''
   def decrypt(ciphertext, key):
    plaintext = ''
    for letter in ciphertext:
        letter = letter.lower()
        if letter != ' ':
            index = letters.find(letter)
            if index == -1:
                plaintext += letter
            else:
                new_index = (index - key) % num_letters
                plaintext += letters[new_index]
        else:
            plaintext += ' '
    return plaintext
   '''

## Encrypting and Decrypting Messages

In this project, I have included a Python file called `caesarcipher.py` that allows you to encrypt and decrypt messages using a specific algorithm. To use this feature, follow these steps:

1. Open the terminal or command prompt.
2. Navigate to the project directory: `cd PRODIGY_CS_01`
3. Run the `casercipher.py` file: `C:\Users\tgrac\OneDrive\Desktop\Cybersecurity\caesarcipher.py`
4. Follow the prompts to enter the message you want to encrypt or decrypt.
5. The program will output the encrypted or decrypted message.


## Output

![Screenshot (455)](https://github.com/GraceAdvitiya/PRODIGY_CS_01/assets/137154095/c892c013-0f3e-467a-bbb2-369192dad30b)


Happy coding!
