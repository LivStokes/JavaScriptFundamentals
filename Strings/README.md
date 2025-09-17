# Strings

I created a string by surrounding a word or sentence with double quotes. But I can also use single quotes.

* let sentence = 'The quick brown fox jumped over the lazy dog'

# String Objects

When you create a string in JavaScript it is converted into a data type called a string object. 
An object in JavaScript can not only store data, it can also be used to manipulate the data. What do I mean by that? Well, it has a series of properties and methods that we can use.

e.g. of a property;
- sentence.length

By using dot length, we get the value 44. That is the number of characters in the sentence, ‘The quick brown dog jumped over the lazy dog’

e.g. of a method;
- sentence.startsWith('The')

Now we’re asking if the string we’ve called sentence, starts with the string ‘The’. We get the answer True.

- True and False are special kinds of number, called a Boolean, we’ll see much more of them later.

The string object has lots of methods, one lets us convert each letter to lower case.

- sentence.toLowerCase().startsWith('the')

Now we get true. See how we can chain together the methods. Here, up to the first dot, sentence starts with an upper-case T. Then we use the method toLowerCase, so after the second dot the string now starts with a lower-case t. When we ask if sentence starts with the, with a lower case t, the answer is true.

Often in code, you’ll want to search through a string to see if it has a particular sequence of characters. 

As well as startsWith, there is also endsWith.
- sentence.endsWith('dog')
Is true, but

- sentence.endsWith('lazy')
is false

if the word you’re searching for is in the middle of the string. Then you can use includes.
- sentence.includes('fox')
The answer is true. In programming speak we say the method returns true.

# indexOf Parameters

To know where the word ‘fox’ is in the sentence? Then we use
- sentence.indexOf('fox')
Which returns 16, 

If we start from the beginning and count the letters, including the spaces, We find ourselves on the space before the word fox. That is because the first letter isn’t index one, it is index zero. We can show it in the console using
- sentence[0]
Which shows the single character at position zero. t.

If we swap zero to 16, 
- sentence[16]
we get f at the beggining of fox.

Add another string to the string using +=
- sentence += ". If the dog barked was it really lazy?"

+= is the same as sentence = sentence + '. If the dog barked was it really lazy?'
* 'The quick brown fox jumped over the lazy dog''. If the dog barked was it really lazy?'

When we used the method indexOf, we included the word ‘fox’ in the brackets. All methods use brackets, it sets them apart from a property such as length that doesn’t need brackets

The word we supplied is called a parameter.
The indexOf method is most often used with a single parameter like this, but we can use a second parameter.

The sentence now has two examples of the word ‘dog’. If we use 
- sentence.indexOf('dog')
Then we get the return value 41. Which is the position in the string of the first ‘dog'.

Suppose we want to find the position of the second ‘dog’. Then we add a second parameter, set to one more than the value previously returned. 
If the second parameter is 41 then the return value is 41. We’re setting the position in the string to start the search from, and it finds the word ‘dog’ immediately. 

If instead we set it to 42, then the return value is 53. This is where we find the second ‘dog’.
- sentence.indexOf('dog', 42)

# SubString

To extract part of a string we can use the method substring.
- sentence.substring(53) 
"dog barked was it really lazy?"

This will return everything in the string sentence, from the character at position 53.

We can use two parameters. If we do the second parameter is the end index, where to stop accessing the string sentence. What value should we use to get the value ‘dog’ return?
- sentence.substring(53, 56)

{
    let sentence = 'The quick brown fox jumped over the lazy dog';
    <
    sentence += ". If the dog barked was it really lazy?"
    < "The quick brown fox jumped over the lazy dog. If the dog barked was it really lazy?"
    sentence.substring(53)
    < "dog barked was it really lazy?"
    sentence.substring(53, 56)
    < "dog"
}

We can access a sub string from the sentence using a different method, slice. At first it seems identical to substring.
- sentence.slice(53, 56)

Where it differs is when we use minus values for parameters.
- sentence.slice(-5, -1)
Returns 'lazy'

A minus parameter will start at the end of the string and count backwards. Do this with the method substring and you get an empty string returned, because all parameter values below zero are changed to zero.
- sentence.substring(-5, -1)
Becomes
- sentence.substring(0, 0)
With a start and end index of zero we get no characters returned.
