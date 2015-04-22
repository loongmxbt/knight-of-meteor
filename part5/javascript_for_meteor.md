# A JavaScript Primer For Meteor

JavaScript is a language full of contradictions: it’s named after Java even though it doesn’t have anything to do with it, it was [created in 10 days][#javascript-histtory] but is still in use 20 years later, and despite getting its fair share of criticism, it’s ubiquitous on the web.

If JavaScript has one thing going for it, is that it’s easy to get started with. Now don’t get me wrong: truly mastering JavaScript is a difficult task. But learning enough to get by isn’t that hard, and shouldn’t take long especially if you already have some experience with other programming languages.

What’s more, when building Meteor apps you’ll often find yourself re-using the same patterns over and over. And as stated by the Pareto principle, learning 20% of a language should be enough to cover 80% of situations.

So today, let’s take a look at the absolute minimum amount of JavaScript you need to know to learn Meteor.

### Following Along

Did you know that you already possessed a full-fledged JavaScript development environment? I’m talking about the very browser you’re reading this with! (Unless you’re using Lynx I guess. Sucks to be you.)

So you can follow along with all these examples simply by typing them into your browser console. Here’s a handy guide on how to open it in various browsers.

Ready? Let’s learn some JavaScript!

### Variables

Here’s how you declare a variable in JavaScript:

var a;
The var keyword lets JavaScript know that whatever comes after is a variable. Now let’s assign a value to our variable:

var a = 12;
Now maybe you’ve seen something like this while looking at some JavaScript code:

a = 12;
JavaScript doesn’t seem to mind when you ommit the var keyword. So what is it good for?

The var keyword makes our variable local. Inside a Meteor app, this means that prefixing a variable with var will restrict its scope to the function you’re declaring it in (or the file, if you declare it outside of any function).

On the other hand, omitting the var keyword will make your variable available to your whole Meteor app. Sometimes that’s good, but in most case it’s better to try and avoid polluting the global scope.

### Functions

Here’s how you declare a function in JavaScript:

var myAwesomeFunction = function (myArgument) {
  // do something
}
And here’s how you’d call your function:

myAwesomeFunction(something);
You’ll notice function declarations follow the same var something = somethingElse pattern as variable declarations.

As they should, since in JavaScript, functions are variables too! This means that you can do stuff like using functions as arguments for other functions:

square = function (a) {
  return a*a;
}
applyOperation = function (f, a) {
  return f(a);
}
applyOperation (square, 10); // 100

### Return

A return statement takes a value and returns this value as the result of a function. The key thing to remember here is that whatever comes after return will never get executed:

myFunction = function (a) {
  return a * 3;
  explodeComputer(); // will never get executed (hopefully!)
}

### If Statements
Here’s what an If statement looks like in JavaScript:

if (foo) {
  return bar;
}
As long as the block of code inside the if fits in one line, you can also use this shorthand syntax (note the lack of curly brackets):

if (foo)
  return bar;
  
### If/Else Statements
Here’s what an If/Else statement looks like in JavaScript:

if (foo) {
  function1();
} else {
  function2();
}
If/Else statements also have their own shorthand syntax:

foo ? function1() : function2();
This is particularly useful when assigning a value to a variable:

var n = foo ? 1 : 2;
This means “if foo is true, then set n to 1, otherwise set it to 2”.

Oh and for good measure, here’s an If/Else If/Else:

if (foo) {
  function1();
} else if (bar) {
  function2();
} else {
  function3();
}



[#javascript-histtory]:https://www.w3.org/community/webed/wiki/A_Short_History_of_JavaScript