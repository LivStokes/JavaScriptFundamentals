# Strings

I created a string by surrounding a word or sentence with double quotes. But I can also use single quotes.
let sentence = 'The quick brown fox jumped over the lazy dog'

# String Objects

When you create a string in JavaScript it is converted into a data type called a string object. 
An object in JavaScript can not only store data, it can also be used to manipulate the data. What do I mean by that? Well, it has a series of properties and methods that we can use.

e.g. of a property;
sentence.length

By using dot length, we get the value 44. That is the number of characters in the sentence, ‘The quick brown dog jumped over the lazy dog’

e.g. of a method;
sentence.startsWith('The')

Now we’re asking if the string we’ve called sentence, starts with the string ‘The’. We get the answer True.

- True and False are special kinds of number, called a Boolean, we’ll see much more of them later.

The string object has lots of methods, one lets us convert each letter to lower case.

sentence.toLowerCase().startsWith('the')

Now we get true. See how we can chain together the methods. Here, up to the first dot, sentence starts with an upper-case T. Then we use the method toLowerCase, so after the second dot the string now starts with a lower-case t. When we ask if sentence starts with the, with a lower case t, the answer is true.

Often in code, you’ll want to search through a string to see if it has a particular sequence of characters. 

As well as startsWith, there is also endsWith.
sentence.endsWith('dog')
Is true, but

sentence.endsWith('lazy')
is false