---
title: Object, Array and Function
layout: lesson
description: Lesson 2
prev: lesson1.html
---

In the previous lesson we have seen the main _JavaScript_ types. In this lesson we are going to analyse in-depth the _Object_ type and its subtypes.

## Object

>Object refers to a data structure containing data and instructions for working with the data. [[MDN](https://developer.mozilla.org/en-US/docs/Glossary/Object)]

In other words and _Object_ is a data container that usually is a representation of a real-world thing, like an animal.

```js
const penguin = {
    name: 'Penguin',
    habitat: 'South Pole',
    height: 110
    pic: '🐧'
}
```

Each name/value pair is called _property_ (eg. `name: 'Penguin'`).

All the _properties_ must be wrapped in _curly brackets_ and separated by _comma_.

An _Object_ property can contain any kind of value, like `string`, `number`, `boolean` or even another `object`.

To **get** the value of a property from an object you have two options:

The _dot notation_
```js
penguin.height // 110
```
Or using _square brackets_
```js
penguin['height'] // 110
```

In a similar way you can also **set** a _property value_:
```js
penguin.height = 100

penguin.height // 100
```

or

```js
penguin['height'] = 100

penguin['height'] // 100
```

## Array

> An array is an ordered collection of data (either primitive or object depending upon the language). Arrays are used to store multiple values in a single variable. This is compared to a variable that can store only one value. [[MDN](https://developer.mozilla.org/en-US/docs/Glossary/Array)]

In _JavaScript_ an Array is a special type of _Object_. The main purpose of an _Array_ is to store ordered data.
Let's imagine to want to store some animals ordered by height. Using normal _Objects_ would be difficult to have a quick way get the fastest one.
_Array_ to the rescue.

```js
const animalsOrderedByHeight = [
    {
        name: 'Elephant',
        habitat: 'Savannah',
        height: 300,
        pic: '🐘'
    },
    {
        name: 'Penguin',
        habitat: 'South Pole',
        height: 110
        pic: '🐧'
    },
    {
        name: 'Cat',
        habitat: 'Sofa',
        height: 25,
        pic: '🐱'
    }
]
```

All the _Array items_ must be wrapped in _square brackets_ and separated by _comma_.

An _Array item_ can contain any kind of value, like `string`, `number`, `boolean`, `object` ore even another `array` (multi dimensional _Array_).

Each _item_ in the _Array_ have an **index** starting from **0**.

To **get** a value out of an _Array_ you need to know its **index**.

```js
const elephant = animalsOrderedByHeight[0]
const cat = animalsOrderedByHeight[2]
```

In a similar way you can also **set** an _item_

```js
animalsOrderedByHeight[3] = {
    name: 'Snail',
    habitat: 'Most of the world',
    height: 1,
    pic: '🐌'
}
```

Now combining what we learnt previously about retrieving an _Object_ property

```js
animalsOrderedByHeight[3].name // 'Snail'
```

Of course we have a lot of powerful tools to work with _Objects_ and _Arrays_ in _JavaScript_, but we need first to introduce the concept of _Function_.

## Function