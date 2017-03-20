# Homework #4

## Instructions
---
1. Feynman Writing Prompts - Write out explanations of the following concepts like you are explaining it to a 12 year old.  Doing this will help you quickly discover any holes in your understanding.  Ask your questions on Slack.
		
	* Q: Callback Functions

	A: A callback function f() is a function that is send as an argument to the parameters of another function p(). 
	Ex: f(p);
	Function f() can call the function p() in its body of statements.

	* Q: Closure

	A: A Closure is a function i() that was returned by a function o(). The specific of i() is that it remembers the place (state) from which it came. As for exemple it remembers and is able to use the variables which the function o() had outside of i() when it returned it.

	* Q: arguments array

	A: A function f() can be called with one or more arguments even if the f() declaration didn't have parameters. Those arguments can be accessed as an array using keyword 'arguments'.
	Ex: 
	function f() {
		for(var i = 0; i < arguments.length; i++) {
			console.log(arguments[i]);
		}		
	}

	f(1,2,3,4,5);


	* Q: recursion

	A: Recursion is a way of program execution when a function is calling itself in its body of instructions. This has a downside beeing prone to error of ifinite loop, as at some point the recursive calling has to stop.
	Ex: 
	function f(x) {
	if(x <= 0) return x;
 		f(x - 1);	
	}

	* Q: prototype

	A: A prototype is a function that is defined for a class of objects and will be available for each object of that class. We use keyword 'prototype' to do that.
	Ex: Let's say we take an existing class like 'String'.
	String.prototype.printToConsole() = function () {
		console.log('This is a prototype');
	}
	Then we can call String.printToConsole();
	Instead of String you can use any predefined class or a class you defined.

	* Q: constructors

	A: Constructors are a special function used to instantiate an object of a class. We use keyword "new" before the call of the function.
	Ex: 
	function Dog(properties) {
		this.name = properties.name;
		this.numbeOfLegs = properties.numberfLegs;		
	}

	var dog1 = new Dog({name: 'Doggy', numberOfLegs: '4'});



2. Fork and clone this repo.  When you need to commit use the following commands.
		
	* git status
	* git add --all
	* git status
	* git commit -m "your commit message"
	* git push origin master

3. Install dependencies using `npm install`.  Run tests using `npm test`.

4. Make the tests pass!



#### Congratulations on finishing Homework #4!
Apply to our full-time or part-time immersive program to learn cutting edge technologies that are used by top technology companies around the world.

Our part-time and full-time courses are 13 intense weeks of focused study on the most relevant technologies.  

Class sizes are small to ensure that each student gets individual attention from our world class instructors to help them succeed.  We also provide career support both during and after the course to help you succeed.  We are committed to your success.

For more information visit: https://www.lambdaschool.com
