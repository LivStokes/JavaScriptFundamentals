# Function definition

A function is a series of lines of code in a block. 
To call a fuction, provide the name of the function followed by bracets.
Values between the bracets are called parameters.
A function can optionally return a value.

To create a function use:
keyword function, function name, opening bracket
function functionName {

}

When using paraments:
function functionName (parameter a, parameter b) {

}
This is the function defenition.

 At this stage we’ve entered the area where we add our JavaScript code. If the function returns a value, then we use the keyword return. This can optionally be followed by JavaScript code. When the running program encounters the word return, it will exit the function and return to wherever the function was called.

A few examples will help enormously.
function multiply( a, b ){
   return a * b;
}
multiply(2,3)

answer = 6.

A function is creating a block of code statements that do a useful job and that we can reuse many times.
The methods: String object, toLowerCase, startsWith, indexOf etc. are all functions. 

# Converting Angles

Angles are in radians not degrees
A full revolution in radians is 2π.

To create a functinon that will convert degrees to radians

function degToRads(angle){
   const pi = 3.1416;
   return angle / 180 * pi
}

Asterisk for multiplication.
Forward slash for division.

Full revolution is 2π.
Half revolution is π.

degToRads(180)
< 3.1416

degToRads(90)
< 1.5708

Here 180 is a half revolution in degrees and the function returns the approximate value for π that we used in the function.

the constant pi can only exist for code insie the function.
It is described a local to the function. Called a scope.

# Converting distance

function milesToKilometres(distance){
   const miles = 1.609; // 1 mile = 1.609 km
   const kilometres = distance * miles;
   return kilometres;
}

console.log(milesToKilometres(10)); // 16.09

OR

function milesToKilometres(dist) {
    return dist * 1.609;
}

milesToKilometres(5)
< 8.045

To get a more precise number = use JavaScript object. Just like a string the Number object has several methods.
One is a function that will convert the number to a string with a specied number of digits following the decimal point.

function milesToKilometres(dist) {
    return (dist * 1.609).toFixed(1);
}

milesToKilometres(5)
< "8.0"

" " means that return value is a string. 
We want it to be a number. So edit like this:

Number((dist * 1.609).toFixed(1));

function milesToKilometres(dist) {
    (return dist * 1.609).toFixed(1);
}

How this works:
The JavaScript execution will start with
dist * 1.609 = 8.045
Then we convert 8.045 into a string rounding the value to a single decimal place.
(8.045).toFixed(1) = "8.0"
Finally using Number we convert this String value back into a numeric value.
Number("8.0") = 8
