# 0x04. UTF-8 Validation

## Overview
This project contains a task related to determining if a given data set of UTF-8 encoded strings are valid.

UTF-8 is a common character encoding that uses variable width encoding to store text in binary data.

Some properties of UTF-8 encoding:
- ASCII characters use 8-bit encoding (1 byte)
- Extended ASCII characters use 16-bit encoding (2 bytes) 
- Characters in languages like Chinese, Japanese, etc use 24-bit encoding (3 bytes)

## Task

### 0. UTF-8 Validation

- File: [0-validate_utf8.py](0-validate_utf8.py)

- Description: This task involves developing a method to determine if a given data set contains valid UTF-8 encoded strings.

The data set is provided as a list of strings representing each string's corresponding bytes as decimal integers.

The implementation should validate the following:

1. Each integer maps to a valid UTF-8 byte
2. The integers represent a valid UTF-8 encoding of some string

The method should return True if the data set contains only valid UTF-8 strings, else False.

This task covers:
- Understanding UTF-8 encoding rules
- Validating integer byte values match UTF-8 binary patterns 
- Implementing logic to analyze lists of integers as UTF-8 encoded strings

## Tasks To Complete

+ [x] 0. **UTF-8 Validation**<br/>[0-stats.py](0-stats.py) contains a script with a function that determines if a given data set represents a valid UTF-8 encoding:
  + Prototype: `def validUTF8(data)`.
  + Return: `True` if data is a valid UTF-8 encoding, else return `False`.
  + A character in UTF-8 can be 1 to 4 bytes long.
  + The data set can contain multiple characters.
  + The data will be represented by a list of integers.
  + Each integer represents 1 byte of data, therefore you only need to handle the 8 least significant bits of each integer.

