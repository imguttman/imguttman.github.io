---
layout: post
title: "Ruby Classes: Why, When, and How"
date:   2015-01-04 12:30:00
categories: blog
---
Classes “group behaviors (methods) into convenient bundles, so that you can quickly create many objects that behave essentially the same way” (WGB, pg. 61). The objects created from the Class are called instances of that Class. Ruby has its own built-in classes (String, Object, Class, etc.) but also allows you to create your own custom classes.
HOW: Use a constant - a special type of identifier in Ruby whose value doesn’t change over time - to name and define a class. To manufacture an instance of that class, call the new method (this type of method is called a constructor).

The data associated with an instance is known as the instance’s state. This data is held in instance variables - a type of variable that begins with an ‘@‘ sign and is only visible to the object to which it belongs. Instance variables come into existence through methods. Classes have access to a special method - #initialize - that gets executed each time an instance of the class is created. The initialize function sets a baseline state for your class instances.

To clean up a class/make it more readable, consider using attr_* method family. An attribute is a high level term to describe a property of an object. The attr_* method family functions as a shortcut that creates an instance variable and automatically wraps that instance variable into a method.

 WHEN/WHY: Writing or reusing custom classes in ruby allows a programmer to specify and share characteristics across numerous objects. As a primary source of the objects that will inhabit your program, classes play a large role in determining the make-up of your program’s virtual world. As Sandi Metz explains, the number and cohesion of an application’s classes will “constrain the imagination of everyone downstream.” Ultimately, Metz says, classes in an applications serve to “[construct] a box that may be difficult to think outside of.” Knowing the impact that classes will have on a program helps to explain why it’s important to have classes with a single responsibility.  A class with more than one responsibility is difficult to reuse, making it difficult for our code to remain changeable and maintainable.
