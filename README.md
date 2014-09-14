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
##Implicit Vs Explicit
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
