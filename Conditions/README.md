# Conditions

We’re going to enter a new function; we’ll call it ‘compare’ and it has two parameters, a and b.
<script>
    function compare(a, b){
        
}
</script>

Keyword, if, follows the {} brackets.
Inside the brackets must evaluate to a Boolean. 
Meaning whatever we enter inside the brackets has to be either true or false. 
e.g. enter a is less than b. Following the closing bracket, we enter curly braces. Strictly speaking, if we only have a single line following the brackets then we don’t need curly braces. But highly recommend you always use them

<script>
    function compare(a, b){
        if (a<b){
            console.log('a is less than b');
        }
    }
</script>

compare(10, 20)

10 is less than 20, so the statement inside the brackets is true and so the program moves to inside the curly braces. 
This prints the line a is less than b in the console.

compare(20, 10)
Prints undefined because it is not true.
So we create the if/else function.

<script>
    function compare(a, b){
        if (a<b){
            console.log('a is less than b');
        }else{
            console.log('a is greater than b')
        }
    }
</script>

compare(10, 10)
Prints a is greater than b.


