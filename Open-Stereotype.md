# Open-Stereotype
Open-Stereotype is a way to store information. Once recognized via Open-Vision, we have to dynamically create classes, object, and inheritance.

# Human way to think
First of all, before coding anything, we need to know what is the idea behind the project. 

How does humans thinks? Why does humans have stereotypes? What is a stereotype? Do we need them? We will try to answer thoses questions here. 

It could looks off topic or philosophic, but when we talk of a machine which speak and think we need a model. 
What else to choose than model chosen by life on earth, chosen by Trial/Error after billions of years. 
This is the model of life I want to show you/explain to you. 
Obviously, I am not a philosopher, I have one way to think and you can share your way to do it. 

It is said we have an advice of people only seconds after seeing them. 
This is caused by stereotypes. We always thought that stereotypes were negative. 
But what is a stereotype? Everyone knows that `I do not like [Insert etnic or religion]` is a stereotype.
A stereotype -in this case- is much more than this, it also say : 
* `This is a human`
* `This is a duck` 
* `Ducks does 'Kwak kwak'`
* `A door is something on houses we use to go in or go out`
* `We can knock knock at the door and someone will come to open, or else we can turn the latch`.
* `Open a close door when we are not authorized to is a crime`

Are stereotypes needed? Imagine your program, every object you create needs some methods and attributes. 
Now, imagine you need to create a new objec with every properties each time you encounter a new object. 
Even if you do not have the information, you will need to save it and store null values. 
Even with the null value, the whole RAM will be used. 
Even if you recognize the item once, you will remember its color, methods and more useless things. 
`But this the way the life have chosen!`. Really? 
Do you remember what you have eaten one month ago? 
The life have chosen to keep only our interests. 
Then, when you see a door, you just say `It is a generic door` and do not instanciate any more door.
This is exactly what a stereotype is, a way to compress data by inheritance. 
This is what we will create here.

# Guidance

The main words to remember are : 
* Inheritance
* Modularity

## We instanciate only parents items, in READ ONLY
The parent item is always in read only. 
When we encounter things multiple times, it could be good to merge singularities -local items- into the parent. 
In this way, the AI will learn slower but better. We can have 3 doors pointing to the parent door. 
If the 3 doors can be open with the latch, we can say every doors can `potentially` be open by the latch.

## Memory is precious (aka Garbage collector)
If an item is like the parent, DESTROY IT. If an item is not seen a while ago, store it in long term memory. If a long term item is not seen a while ago, DESTROY IT.

## Null is lost
A null item can NOT be instanciated. Instead, instanciate a generic item pointing to the parent and to local memory. 
The local memory will be for this item and is basicly NULL. 
Than, the object is only the size of two addresses. 

## Local data
The local data of a single instanciated object -singularity- can rewrite parents methods and properties

# Implementation

## Generic Data Structure

| Generic Data Structure |
| ---------------------- |
| Pointer to Parent data |
| Pointer to Local data  |

## Parent Data Structure

| Parent Data Structure              |
| ---------------------------------- |
| Unique pointer to Parent structure |
| Array of method pointers           |
| Array of BIG attribute pointers    |
| Array of attributes                |

## Local data Structure

| Parent Data Structure              |
| ---------------------------------- |
| Unique pointer to Local structure  |
| Array of method pointers           |
| Array of BIG attribute pointers    |
| Array of attributes                |

## Structure of data structure

| Structure of data structure |
| --------------------------- |
| Number of methods           |
| Number of BIG attributes    |
| Number of attributes        |
| Type of attributes          |
| Name of attributes          |

# Contribute
As the project is open, feel free to contribute by opening an issue, make a pull request or contacting me via mail [alexis.paques@gmail.com](mailto:alexis.paques@gmail.com) or Skype (penegalexis)

# License
This work, documentation and ideas included are given under GNU GPLv2 license.

# Credits
Alexis Paques (@AlexisTM)