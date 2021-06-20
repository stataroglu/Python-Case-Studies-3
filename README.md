
# Python-Case-Studies-3


## Task 1. Encode and decode some text

Suppose you have a message in English of a sufficient length, say 100 charachters. The goal of this task will be to turn that text into a list of integers, encode it by applying an operation on the indexes, and then decode it back to reproduce the original message. You can think of this as an exercise in making a message secret by encoding it and then decoding it.

The following string contains all of the printable characters found on most keyboards, so it can be used for turning the message into integers:

```python
all_char = string.printable
```

so that letter 'c' corresponds to index `12` in `all_char`. 

In the cell below, write a piece of code that will do the following work:

* (1) Introduce a message to work with (a string of English text, should be from 50 to 100 charachters). 
* (2) Create a list with symbols from your message. For example, the message `secret` becomes the list `[28, 14, 12, 27, 14, 29]` in terms of the list `all_char`.
* (3) Now encode the message by incrementing the integers in the list by a number, e.g, 10, so that your secret list from above becomes `[38 24 22 37 24 39]`. The encoding number is a `key` that can be used to decode it.
* (4) Now add to this list the key as the last element, so that your list becomes in the examle above `[38 24 22 37 24 39 10]` 
* (5) Print the encoded array
* (6) Write a piece of code to decode the message using the key 
* (7) Now assume that you do not know that the last element in the array is the key, but you do wish to read the message. You also know how the message was encoded (all integers shifted by some number). Assume that the secret message is likely to contain common English words 'the', 'and', 'have'. Write a piece of code that uses this condition to guess what the value of the key is. 
* (8) Print the decoded message. 


