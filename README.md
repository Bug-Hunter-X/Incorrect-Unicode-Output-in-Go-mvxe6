# Incorrect Unicode Output in Go

This repository demonstrates a common issue in Go programs when dealing with Unicode characters. The problem lies in how the program handles character encoding, leading to potential output discrepancies across different systems.

## Bug Description

The program attempts to print the string "Hello, 世界".  However, if the system's default encoding is not properly configured to handle UTF-8, the output might be garbled or show unexpected characters.

## Solution

The solution ensures that the program explicitly uses UTF-8 encoding for both input and output. This guarantees consistent output regardless of the system's default encoding.