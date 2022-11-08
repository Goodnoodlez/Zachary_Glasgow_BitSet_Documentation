# Zachary_Glasgow_BitSet_Documentation

## Introduction
Bitset is an array of boolean values that are stored as either 0 or 1 whit 0 being false and 1 being true. Each Boolean value is stored in the same area optmized for storage space. Each Boolean value is stored in one bit so each Bitset value takes up less space than a normal bool or vector. Traditional bool values take up sixteen bits this is the same as 16 bitset values that functionaly do the same work.

## Uses of BitSet
Bitset should be used whenever memory could be an issue for whatever machine the code is being ran on. This is due to the miniscule memory required for BitSet to be implmented. A real world implementation that you might actually see is on any true false survey that is might recieve an abundance of people answering. If a BitSet is used on the check if their is twenty questions you would only need twenty bits of storage to store the data that is recieved from the survey. If a Bool was used in place of the Bitset for the twenty question you would need 320 bits for every completed survey. On a small scale the difference might be negligble but as you scale to larger numbers of people answering the more taxing the difference in the two types of functions becomes vast.

## Implementation of BitSet
BitSet is part of the standard library in C++ which means that you dont need to include any external library to use it. To use Bitset you first must know how big of a set you want to use since it is intialized at the start of running your program. For example to refer back to the survey example that was given previously on intializatoion of the BitSet you haved to know the number of querys given in the survey which would be twenty in the current use. BitSet will not work if you were to try and change the number of querys as the program was running. This is the major drawback of BitSet but as long as you know the number of of querys then the problem is moot.

## How to use BitSet
These are the common functions you might use while using BitSet.

bitset<8> set8; This implments a bitset named set8 that has 8 querys that can be used its intial value being 00000000

set8.set(0); This changes the value of the bit in the zero position to 1 changing the set to 00000001

set8.rest(0); This changes the value of the bit in the zero position to 0 changing the set to 00000000

set8.flip(); This changes the value of the whole set to the oposite value changing the set to 11111111

set8.size(); This reports the size of the bitset which would currently be 8

set8.to_string(); This converts the value of the bitset to a string which would read out currently "11111111"

## Conclusion
BitSet is very useful way to store any data that can have a true or false value Since it has a small size and does the same job as its competitors.
