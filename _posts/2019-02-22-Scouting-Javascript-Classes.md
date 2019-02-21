---
layout: post
title:  "Scouting Javascript Classes"
date:   2019-02-14
excerpt: "A Beginners View of Classes Through a Moon Prism"
image: "https://i.ibb.co/4f12rsK/Scouting-Class.png"
---
Inspired by a conversation I heard yesterday I wanted to give a clear explaination of object-oriented JavaScript and _classes_. The first "space-time" key to understand classes is to understand _object literals_. You may be aware that code can be used to describe both abstract and real world objects. Object literals are a way of encapsulating data in a neat single package through key-value pairs of _properties_ and _methods_. Since enhanced object literals have come into play with ES2015, it is even easier to create them. 

![Luna and Artemis](https://i.ibb.co/VSBbrGz/lunaandartemis.jpg#feature)

So, this is going to sound crazy, but the overheard conversation was between two cats talking about a magical heroine. Let's see if I can describe her as an object literal. 

    const sailorMoon = {
      humanName: 'Usagi',
      nickName: 'Meatball Head',
      birthday: 'June 30',
      age: 14,
      favoriteAnimal: 'Rabbit',
      favoriteColor: 'White',
      favoriteFood: 'Ice Cream',
      strength: 'Loyalty',
      weakness: 'Thunder',
      phrase: function() {
        console.log('Moon Prism Power Makeup!')
      }
    }

Notice that our heroine's object literal is arranged within curly brackets and key-value pairs are separated with a comma. All of the key-value pairs are "properties" of ```const sailorMoon```. The last pairing is called a "method".

![Sailor Scouts](https://i.ibb.co/rGYJDQ0/Senshi-Sailor-Moon.jpg#feature)

Our Sailor Moon object literal is all well and good, but imagine my astonishment on learning there were four other magical Sailor Scouts! There must be a quicker way to build our Sailor Senshi team than writing out the same object literal keys every time a new one magically makeups! Thanks to ES2015, yes there is! Classes in JavaScript are lovely syntatical sugar waving a moon crescent wand over object creation and inheritance issues.

With class, we can make a Sailor Scout blueprint and churn out four, five, even nine scouts with a few lines of code. Moon Cosmic Dream Action!

![Outer Sailor Scouts](https://i.ibb.co/NpWmxV3/Outer-Senshi.jpg#feature)

Let's start with declaring our class. Notice the name of the class is capitalized. This is common convention to deliniate a class.

    class SailorScout = {
      constructor() {

      }
    }



