# Simple File Encryption & Decryption with Node.js Streams

## Description

This is a lightweight Node.js application that demonstrates file encryption and decryption using Node.js Streams. It processes files in a memory-efficient way by reading data in chunks, applying a simple transformation, and writing the output to a new file.

## Features

- Uses Transform Streams to modify file data on-the-fly.

- Efficient stream-based processing (no need to load entire files into memory).

- Simple byte-shifting encryption (increments each byte except 255).

- Reversible decryption (decrements each byte except 255).


## Installation

Make sure you have Node.js installed on your system then, clone this repository

## How It Works

🔒 Encryption (encryption.js)

- Reads read.txt in chunks.

- Increments each byte (except 255) to transform the content.

- Writes the transformed data to write.txt.


🔓 Decryption (decryption.js)

- Reads write.txt (the encrypted file) in chunks.

- Decrements each byte (except 255) to restore the original content.

- Writes the restored data to decrypted.txt.


  ## 📝 Notes

- The encryption logic shifts each byte by +1, and decryption shifts it back by -1.

- This is a basic encryption method, meant for educational purposes.

- The program uses Node.js built-in modules (fs, stream), making it lightweight and dependency-free.
