---
layout: post
title:  "Scouting Javascript Classes"
date:   2019-02-14
excerpt: "A Beginners View of Classes Through a Moon Prism"
image: "https://i.ibb.co/4f12rsK/Scouting-Class.png"
---
Inspired by a conversation I heard yesterday I wanted to give a clear explaination of object-oriented JavaScript and **_classes_**. The first "space-time" key to understand classes is to understand **_object literals_**. You may be aware that code can be used to describe both abstract and real world objects. Object literals are a way of encapsulating data in a neat single package through key-value pairs of **_properties_** and **_methods_**. Since enhanced object literals have come into play with ES2015, it is even easier to create them. 

### Object Literal

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

Notice that our heroine's object literal is arranged within curly brackets and key-value pairs are separated with a comma. All of the key-value pairs are **_properties_** of ```const sailorMoon```. The last pairing is called a **_method_**.
We can access different properties or methods of Sailor Moon using _dot notation_ like so:```objectName.propertyKey```.

    console.log(sailorMoon.nickName);
    "Meatball Head"

![Sailor Scouts](https://i.ibb.co/rGYJDQ0/Senshi-Sailor-Moon.jpg#feature)

### Class Constructor

Our Sailor Moon object literal is all well and good, but imagine my astonishment on learning there were four other magical Sailor Scouts! There must be a quicker way to build our Sailor Senshi team than writing out the same object literal keys every time a new one magically makeups! Thanks to ES2015, yes there is! Classes in JavaScript are lovely syntatical sugar waving a moon crescent wand over object creation and inheritance issues.

With class, we can make a Sailor Scout blueprint and churn out four, five, even nine scouts with a few lines of code. Moon Cosmic Dream Action!

![Outer Sailor Scouts](https://i.ibb.co/NpWmxV3/Outer-Senshi.jpg#feature)

Let's start with declaring our class. Notice the name of the class is capitalized. This is common convention. Inside of our class, we will add a **_constructor_** method. The constructor is like a factory that will make all of the property values we request as _parameters_ we place in the _()_. So, what do you think a sailor scout needs? 

    class SailorScout = {
      constructor(scoutName, humanName, birthday, element, favoriteColor, favoriteFood, strength, weakness) {
      }
    }

So we have our constructor and request list. Let's place some object _properties_ in the _constructor_ and link them to our requests or _parameters_. We need to use dot notation and the keyword **_this_**. In this case **_this_** refers to the object being created. It is linked to a property using dot notatation and set equal to a parameter (value).

    class SailorScout = {
      constructor(scoutName, humanName, birthday, element, favoriteColor, strength, weakness) {
        this.scoutName = scoutName;
        this.humanName = humanName;
        this.birthday =  birthday;
        this.element = element;
        this.favoriteColor =  favoriteColor;
        this.strength = strength;
        this.weakness = weakness;
      }
    }




