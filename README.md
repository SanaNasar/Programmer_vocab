## Programmer Vocab

## Varaible declaration and Instantiation
* Parts of a Variable:
	* There is the variable name and it's value. Two parts.
	* The variable's name is what you declare it to be. The value is what you assign to it.
* Variables are Initialized.
* All variables are always given an initial value at the point the variable is declared. Thus all variables are initialized.

* Objects are Instantiated.
* Humans are born. Objects are instantiated. A baby is an instance of a Human, an object is an instance of some Class.
* The act of creating an instance of a Class is called *instantiation (Ta-Da!)*


## params
* The params come from the user's browser when they request the page. For an HTTP GET request, which is the most common, the params are encoded in the url. For example, if a user's browser requested.
* params values can come from the query string of a GET request, or the form data of a POST request, but there's also a third place they can come from: The path of the URL.

As you might know, Rails uses something called routes to direct requests to their corresponding controller actions. These routes may contain segments that are extracted from the URL and put into params. For example, if you have a route like this:

match 'products/:id', ...
Then a request to a URL like http://example.com/products/42 will set params[:id] to 42.

## RESTful API
(REST) Representational state transfer

* Representational State Transfer is an architectural style that abstracts the architectural elements within a distributed system. ...
* A REST API defines a set of functions which developers can perform requests and receive responses via HTTP protocol such as GET and POST.
* The REST API should specify what it can provide and how to use it, details such as query parameters, response format, request limitations, public use/API keys, method (GET/POST/PUT/DELETE)

## Variable instantiation

* Instantiation means to create an instance for a variable, class or object. Initialization means to initiate the same object or class for any purpose.


## Implicit Vs Explicit

* In Javascript, If the function that was called has no explicit return statement, then it implicitly returns the value of *this* - the new object.
* In case of an explicit return statement, the function returns the value specified by that statement, but only if the return value is an Object.
* In Ruby.
	
	
		Implicit return - Ruby returns the last value evaluated,
		so with if/elsif/else, we can be sure we return the right value!
		
    	def comparison(a, b)
     		if (a.field < b.field)
       	 		-1
      		elsif (a.field > b.field)
        		1
      		else
        		0
      		end
    	end
   
        
		Explicit returns - we add "return" all over the code
		
    	def comparison(a, b)
      		if (a.field < b.field)
        		return -1
      		elsif (a.field > b.field)
        		return 1
      		else
        		return 0
      		end
    	end
## SSH (Secure Shell)
*  Stands for "Secure Shell." SSH is a method of securely communicating with another computer.
* The "secure" part of the name means that all data sent via an SSH connection is encrypted. This means if a third party tries to intercept the information being transferred, it would appear scrambled and unreadable.
* The "shell" part of the name means SSH is based on a Unix shell, which is a program that interprets commands entered by a user.
## Pass by value
* "Passing by value" means that you pass the actual value of the variable into the function.

* "Passing by reference" means that you pass the variable itself into the function (not just the value).

This has various consequences, and each is useful in different situations.

[Helpful resource](https://developer.mozilla.org/en-US/docs/Talk:JavaScript/Guide/Obsolete_Pages/Defining_Functions)

##Primitive types
* In computer science, *primitive data type* is either of the following:

	* a basic type is a data type provided by a programming language as a basic 	building block. Most languages allow more complicated composite types to be 	recursively constructed starting from basic types.
	* a built-in type is a data type for which the programming language provides built-in support.
	
*  in JavaScript, they are assimilated to a primitive data type that is both basic and built-in.

Classic basic primitive types may include:

	* Character (character, char);
	* Integer (integer, int, short, long, byte) with a variety of precisions;
	* Floating-point number (float, double, real, double precision);
	* Fixed-point number (fixed) with a variety of precisions and a programmer-selected scale.
	* Boolean, logical values true and false.
	* Reference (also called a pointer or handle), a small value referring to another object's address in memory, possibly a much larger one.

##Mutation
* The process of actually changing a variable’s value over time, within a single context, is called mutation.
* In other words, Mutation refers to the ability of a variable or data structure to change over time.

## Mutation testing
* Mutation testing (or Mutation analysis or Program mutation) is used to design new software tests and evaluate the quality of existing software tests.
* Mutation testing involves modifying a program in small ways.
* Each mutated version is called a mutant and tests detect and reject mutants by causing the behavior of the original version to differ from the mutant.

## Abstraction Principle
* In software engineering and programming language theory, the abstraction principle (or the principle of abstraction) is a basic dictum that aims to reduce duplication of information in a program (usually with emphasis on code duplication) whenever practical by making use of abstractions provided by the programming language or software libraries.
* The principle is sometimes stated as a recommendation to the programmer, but sometimes stated as requirement of the programming language, assuming it is self-understood why abstractions are desirable to use.
* When read as recommendation to the programmer, the abstraction principle can be generalized as the "don't repeat yourself" principle, which recommends avoiding the duplication of information in general, and also avoiding the duplication of human effort involved in the software development process.

## Groupings

		
		1) (1 + 2) * 3;  // 9

		2) 1 + (2 * 3);  // 7
		
* The grouping operators are the things we use to help show what should be evaluated first, as in mathematical problems. We’re saying “evaluate this first, then take the result and do something with it”.
* In the first example we’re saying “first add 1 and 2, then take the result and multiply by 3″, whereas in the second example we’re saying “first multiply 2 and 3, then take the result and add 1″.

## What is a Callback or Higher-order Function?

* A callback function, also known as a higher-order function, is a function that is passed to another function (let’s call this other function “otherFunction”) as a parameter, and the callback function is called (executed) inside otherFunction.
* Here is another classic example of callback functions from basic JavaScript:
		
		var friends = ["Mike", "Stacy", "Andy", "Rick"];

		friends.forEach(function (eachName, index){
		console.log(index + 1 + ". " + eachName); // 1. Mike, 2. Stacy, 3. Andy, 4. Rick
		});
###How it works?
* Because functions are first-class objects in JavaScript, we can treat functions like objects, so we can pass functions around like variables and return them in functions and use them in other functions.
* When we pass a callback function as an argument to another function, we are only passing the function definition. We are not executing the function in the parameter.
* It is important to note that the callback function is not executed immediately. It is “called back” (hence the name) at some specified point inside the containing function’s body.
###What is a closure?
* A closure is an inner function that has access to the outer (enclosing) function’s variables—scope chain.
* The closure has three scope chains: it has access to its own scope (variables defined between its curly brackets), it has access to the outer function’s variables, and it has access to the global variables.
* The inner function has access not only to the outer function’s variables, but also to the outer function’s parameters.
* A Basic Example of Closures in JavaScript: 

		function showName (firstName, lastName) { 
		var nameIntro = "Your name is ";
		    // this inner function has access to the outer function's variables, including the parameter
		function makeFullName () {         
		return nameIntro + firstName + " " + lastName;     
		}
		
		return makeFullName (); 
		} 
		
		showName ("Michael", "Jackson"); // Your name is Michael Jackson
		
###Closures’ Rules and Side Effects

	1. Closures have access to the outer function’s variable even after the outer function returns
	2. Closures store references to the outer function’s variables.
	3. Closures Gone Awry

## Dynamic Dispatch

* The process of selecting which implementation of a polymorphic operation (method or function) to call at runtime.
* Dynamic dispatch contrasts with static dispatch in which the implementation of a polymorphic operation is selected at compile-time.
* The purpose of dynamic dispatch is to support cases where the appropriate implementation of a polymorphic operation can't be determined at compile time because it depends on the runtime type of one or more actual parameters to the operation.

[Dynamic Dispatch](http://en.wikipedia.org/wiki/Dynamic_dispatch)


## Protocols

* In object-oriented programming, a **protocol or interface** is a common means for unrelated objects to communicate with each other. These are definitions of methods and values which the objects agree upon in order to cooperate.

[Protocol (Object-Oriented Programming)](http://en.wikipedia.org/wiki/Protocol_(object-oriented_programming))

* A **routing protocol** specifies how routers communicate with each other, disseminating information that enables them to select routes between any two nodes on a computer network.

[Routing Protocol](http://en.wikipedia.org/wiki/Routing_protocol)

## Heap Memory

* The portion of memory where dynamically allocated memory resides (i.e. memory allocated via [malloc](http://stackoverflow.com/questions/1213403/what-is-malloc-doing-in-this-code)).
* Memory allocated from the heap will remain allocated until one of the following occurs:
	* The memory is free'd
	* The program terminates

