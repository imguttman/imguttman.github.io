---
layout: post
title: "Ruby Hashes v. JavaScript Objects"
date:   2015-01-18 12:00:00
categories: blog
---
This week I met JavaScript for the first time. And to keep this metaphor going, I’d say that I was introduced to JS by Ruby. The challenges for the week were designed so that we could “explore the features of JavaScript from the perspective of Ruby.”

When JavaScript through this Ruby lens, I was tempted to project ruby concepts onto my understanding of JS. When I encountered objects in Eloquent JavaScript as “arbitrary collections of properties”, I immediately conflated objects with Ruby hashes.

Hashes are a kind of dictionary of values, where each value is associated with a single key. The key allows you to access its corresponding value in the hash. Objects seem to do the same: an object in comprised of properties. A property is an expression that provides access to a value; properties in objects are written as name:value pairs. A property’s name is just like a variable in that it stores a certain value. Just like hash keys, an object’s property names can “grasp” different types of values (strings, numbers, arrays, booleans, etc).

Despite these similarities on the surface, it’s important to understand that JS objects are not the same as Ruby hashes, and how they’re different. As best I can understand, objects are more accessible (and by extension changeable) than hashes. Objects in JS are comprised of a collection of properties, whereas a Ruby hash is itself a set of variables that reference other objects. In other words, key-value pairs in hashes are more encapsulated than object properties in JS. This is why hashes can be altered only through method calls whereas JS objects can be modified much more easily.
