# Operator and Loops
## For Loops
- repeats until condition evaluates to false
- `for(let i = 0; i < userAttempts; i++){
    let userGuess = prompt('please enter a number 1-100');
    while(userGuess < 1 || userGuess > 100){
        userGuess = prompt('wrong range. go again');
    }`
    
    This for statement makes sure that i is less than the user attempts (not pictured but for class we used 6) and it gives you a prompt of entering a number 1-100. it also initializes i to 0 and adds i everytime you make an attempt.

    ## While Loops
    A while loop executes its statements as long as a specified condition evaluates to true. If it becomes false it will spit out a statement

    Example : `for(let i = 0; i < userAttempts; i++){
    let userGuess = prompt('please enter a number 1-100');
    while(userGuess < 1 || userGuess > 100){
        userGuess = prompt('wrong range. go again');
    }`

    If the userguess is less than 1 or greater than 100 a prompt will come out to make them try again.

## Operators
Assignment Operators

assignment operators or simply "=" 

it assigns whatever is to the right of it to whatever is to the left of it

Example:


`function getuserName(){
   let userName = prompt('please enter your name:');
    console.log(userName);
    user1= userName
    return (userName);
}`

whatever the user puts as their username becomes `user1` and it returns their user name in the webpage.

## Comparison Operators
or simply put "double equal sign" compares whatever is to the right and left of it and makes sure they are **true**

for example: 

    function getuserAnswer(){
    let userAnswer = prompt('DO you like MMA?:')
    console.log(userAnswer);
    
    if (userAnswer.toLowerCase() == 'yes') {
        document.write('<h3>Welcome ' + user1 +'</h3>') ;
    } else {
        document.write('<h3>' + user1 +' , you should try it out</h3>');
    }



in the example its going to compare whatever the users answer is to my question if its a "yes" it spits out a welcome message. if it is something else it will spit out the message try it out. if they answer no for example, the comparison of yes is FALSE.