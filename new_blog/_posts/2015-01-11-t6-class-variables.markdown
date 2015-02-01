---
layout: post
title: "Class Variables Explained"
date:   2015-01-11 12:00:00
categories: blog
---
Class variables defy typical scoping rules in a very useful way.

By appending two @ signs before to a variable name, you can create a class variable that stores information which can be accessed and added to only by class objects and instances of that class. Class variables, usually found in class or instance methods, allow for instances of a class to share information with each other and the class object itself. This expands the potential for classes to more accurately and easily model real-world objects. This visibility for class variables makes them less risky and leaky than global variables and thereby result in cleaner (read: less leaky) code.

Imagine you’re running a dog-sitting service and want an easy way to keep track of the number of dogs that you’re responsible for. You could use a global variable ($dog_count) to solve this problem, making the count accessible and changeable from everywhere in the program. The class variable @@dog_count offers a more sensible alternative. The initialize method might add to this variable each time an instance of the class is created, and then it could be viewed via a class method.

Something to be wary of when working with class variables is the class’s inheritance. “Class variable”, in fact, is sort of a misnomer - it’s more accurate to think of class variables as class-hierarchy variables, because class variables are shared by any subclasses the class might have and instances of those subclasses. This means that class variables found in a class that has many ‘related’ subclasses or parent-classes are more vulnerable to the sort leakiness that deterred us from using global variables in the first place. So, as useful class variables are, they should be used cautiously.
