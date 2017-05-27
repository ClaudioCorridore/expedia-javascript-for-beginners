---
title: If…else, for…in and for…of
layout: lesson
description: Lesson 3
prev: lesson2.html
---

We are almost ready to start writing our first web app, but first, we will need some more tool.

## If…else
As we already say every software starts from some kind of input. But what if we want to trigger different action conditionally to the input value?

For such scenario we can use the **if…else** statement.

> The if statement executes a statement if a specified condition is truthy. If the condition is falsy, another statement can be executed. [[MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/if...else)]

![If…else](assets/ifelse.png)

Let's imagine to have two _variables_ each containing a different hotel _object_ :

```js
const hotelA = {
    name: 'Amazing Luxury Hotel',
    price: 1000
}

const hotelB = {
    name: 'Cool Cheap Hotel',
    price: 200
}
```

and that we want to write a function that, given a _budget_, it returns one hotel that is below that amount :

```js
const getHotelsInUserBudget = function(budget) {
    let result = null;

    if (hotelA.price < budget) {
        result = hotelA
    }

    if (hotelB.price < budget) {
        result = hotelB
    }

    return result
}
```

>**Quiz:** What would be returned by the function if the passed budget is _1_ ?


## For…in

## For…of


[Go to the exercise page](https://jsbin.com/zurijah/edit?js,output)

---
### Further readings

