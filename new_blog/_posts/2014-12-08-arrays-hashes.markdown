---
layout: post
title: "Arrays and Hashes"
date:   2014-12-08 12:30:00
categories: blog
---
TArrays and hashes both store objects (i.e. information) associated with a specific, unique key. Knowing a value’s key enables you to ‘access’ or ‘pull’ (but not remove) that value from the dataset.

With arrays, each item’s key is an integer that corresponds to the item’s position in the array. The first object occupies the zero position, the second occupies position 1, and so on. This sort of inflexibility  - the keys cannot be renamed and update when items are removed or added to the array – makes arrays more well suited for data sets with set orders like rankings. In large datasets, to call a specific item from an array means that you can be certain where that item is listed in an array. So, for example, if you recorded the time it takes for you to run a mile every day for 30 days, stored the times in the array, and then wanted to see you fast you ran on day 15, it would be easy/sensible to know that that time occupies the [14] position in the array (since the first day’s time is found at the [0] place).

Hashes, like arrays, are made up of key-value pairs. The crucial distinction is that with hashes, you have control over both the key and the value of an item. So Hashes are less like lists, and more like a collection of pairs in an abstract cloud stored on your computer. (I know 0% percent about ‘cloud technology’ so hopefully my metaphor doesn’t offend anyone with its imprecision.) Hashes provide us with flexibility, and should be utilized when a dataset has no natural or fixed order. Just because a group of values don’t sensibly fit into a numbered list (read: an array) doesn’t mean it can’t be well organized: Hash keys can store information efficiently with smart labels. Like if we were to store prices of grocery items, it’d be better to have the key be “banana”  rather than a random integer that would be associated with the price of a banana which we’d have to remember (or at least write down (and then remember where we wrote it (can’t you feel the inefficiency of that?))).

(Hashes do abide by an insertion order, which is exactly what it sounds like: the order each item was added to the hash; practically, this tells us the order which items are iterated over.)
