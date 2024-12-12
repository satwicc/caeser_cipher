# Caesar Cipher: Encryption and Decryption in Python

This repository contains Python implementations for both the encryption and decryption processes of the Caesar Cipher. The Caesar Cipher is a simple substitution cipher that shifts characters by a specified number of places in the alphabet.

## Features
- **Encryption**: Encode a plaintext message using a specified shift value.
- **Decryption**: Decode a ciphertext message using the same shift value.

## How It Works
The Caesar Cipher works by shifting each letter in the text by a fixed number of places down or up the alphabet. For example, with a shift of 3, `A` becomes `D`, `B` becomes `E`, and so on. For decryption, the process is reversed.

### Encryption
Given a plaintext and a shift value, the encryption function:
- Converts each character to its ASCII representation.
- Shifts the character within the bounds of the alphabet.
- Leaves non-alphabetic characters unchanged.

### Decryption
Given a ciphertext and the same shift value, the decryption function reverses the shift applied during encryption.

## Requirements
- Python 3.x

## Usage
- Clone the repository:
  ```bash
  git clone https://github.com/satwicc/caesar_cipher.git
  cd caesar_cipher
  ```
- Run the scripts for encryption and decryption.

### Encryption Example
```python
message = input("Enter the Message to be encrypted: ")
shift = int(input("Enter the Shift Value for the Message: "))
ciphertext = ""
for letter in message:
    if letter == " ":
        pass
    else :
        ciphertext = ciphertext + (chr((ord(letter)+(shift-97)) % 26 + 97))
print (encoded_message)

# Example usage
message = "Hello, World!"
shift = 3
ciphertext = encrypt(message, shift)
print(f"Ciphertext: {ciphertext}")
```
### Check out decryption yourself

## File Structure
```
caesar_cipher/
├── caesarshift_encryption.py  # Contains the encryption function
├── caesarshift_decryption.py  # Contains the decryption function
└── README.md   # Documentation for the project
```

## Contributing
- Feel free to fork this repository and contribute improvements or additional features.
- Create a pull request with your changes for review.

## License
- This project is licensed under the MIT License. See the `LICENSE` file for details.

