# JavaScript-Essentials

## What is Global Execution Context ?

## What is Local Execution Context ?

## What is Call Stack ?

## Is javascript multithreaded ?

## Is javascript has asynchronous  execution model?

## What is Event Loop ?

## Callback/Macro-Task Queue? 

## What is Micro Task Queue ?

## Explain setTimout function.

## When our asynchrnously delayed code gets executed ? 

## Pure Functions ?

## High Order Functions ?
   1. copyArrayAndAdd , copyArrayAndMultiply vs copyArrayAndManipulate
   
## CallBack vs High Order fucntion?   

## First Order Function ?

## Are function First-Class Object ?

## Functions are object first rather than function.

## What Is Closure?

## Use Cases of using Closure ?

## Memoization ?

## Prevention from polluting global namespace?

## Lexical/static Scope ?

## Is all variables available at lexical scope are inclosed in function closure ?

## Encapsulate property and fuctions in javascript object.

## Encapsulate property and fuctions in javascript object using dot notation.

## Various ways of creating object in JavaScript. Explain all of them with there downsides and benifites.
``` javascript

   //  Object literal
   
   const user1 = {
   name: "Jack",
   score: 0,
   incrementScore: function(){
           this.score++;
      }
   }
   
   // Dot notation
   
   const user2 = object.create(null);
   user2.name = "Turner"
   user2.score = 4;
   user2.incrementScore = function(){
      user2.score++;
   }
   
   // Using function to remove duplication
   
   function userCreator(name, score){
      const newUser = {};
      newuser.name = name;
      newUser.score = score;
      newUser.incrementScore = function(){
         newUser.score++;
      };
      return newUser;
   }
   
   const user1 = userCreator("Jack", 4);
   const user2 = userCreator("Turner", 5);
   user1.incrementScore();
   

```

## How to lift off shared functions from objects

## Prototypical nature of JavaScript?

## Explain Object.create(commonObject)

## Explain __ proto__ 

## Explain want happens when we call function with new keyword 

## What is Object.prototype ?

## Convert Class syntatic sugar code to ECMAScript 5 
   ```javascript 
      class User {
         constructor(name,score){
         this.name = name;
         this.score = score;
         }
      
         increment(){
            this.score++;
         }
      
      }
      
   let user1 = new User("Jack", 9);
   user1.increment();
   ```
