# Message Encode-Decode Application

A Python-based GUI application to encode and decode messages securely using a key. This app ensures secure communication by transforming messages into encoded formats that can only be decoded with the correct key. It is built with **Tkinter** for the graphical user interface and **base64** for encoding and decoding operations.

---

## Features
- **Encode Messages**: Transform your plain text messages into encoded formats using a key.
- **Decode Messages**: Retrieve the original message using the same key that was used to encode it.
- **Secure Key-Based System**: Messages can only be decoded with the correct key.
- **User-Friendly Interface**: Intuitive design with a clean layout, built using Tkinter.
- **Error Handling**: Displays clear error messages if required inputs are missing or invalid.

---

## How It Works
1. **Encoding**:
   - The app takes a message and a key as input.
   - Each character in the message is shifted by the length of the key.
   - The shifted message is then encoded using the **base64** library.
2. **Decoding**:
   - The encoded message is decoded using **base64**.
   - Each character is shifted back by the length of the key to retrieve the original message.

---

## Project Structure
```
Message Encode-Decode
│
├── Message Encode Decode.ipynb        # The Python script for the application
└── README.md      # Documentation for the project
```

---

## Prerequisites
To run this application, ensure you have Python 3 installed on your system. Additionally, no external libraries are required as the app uses standard Python libraries.

---

## Usage Instructions

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/message-encode-decode.git
   cd message-encode-decode
   ```

2. Run the script:
   ```bash
   python main.py
   ```

3. **Using the Application**:
   - Enter a secure key in the "Enter your key" field.
   - Type your message in the "Enter your message" field.
   - Click "Encode" to encode the message or "Decode" to decode it.
   - The result will appear in the "Result" section.

---

## Example
### Encoding:
- **Key**: `secure`
- **Message**: `Hello World`
- **Encoded Result**: `RUI7H7ZNXzdLUc9O`

### Decoding:
- **Key**: `secure`
- **Encoded Message**: `RUI7H7ZNXzdLUc9O`
- **Decoded Result**: `Hello World`

---

## Contributing
Feel free to fork this repository and submit pull requests with improvements or additional features. Contributions are welcome!

---

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.
