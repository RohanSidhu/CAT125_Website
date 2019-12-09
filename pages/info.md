---
layout: page
title: "Object Oriented Programming"
subheadline: "What is this all about?"
teaser: "When learning anything, one must learn the fundamentals first. This is a fundamental for programming"
permalink: "/info/"
header:
    image_fullwidth: "info.jpeg"
---

*Object Oriented Programming*, or OOP for short, revolves around the idea of having objects. Think simplistically! 


## Simple Objects Like

* Cars
* Animals
* Books
* Food
* Clothes
* ... it goes on


## These objects...

all have something in common. It is that there are multiple types of each of these objects. Cars for instance:

<div class="row">
    <div class="medium-4 columns t30">
    <img src="{{ site.urlimg }}sports.jpeg" alt="">
    </div><!-- /.medium-4.columns -->

    <div class="medium-4 columns t30">
      <img src="{{ site.urlimg }}sedan.jpeg" alt="">
    </div><!-- /.medium-4.columns -->

    <div class="medium-4 columns t30">
      <img src="{{ site.urlimg }}classic.jpeg" alt="">
    </div><!-- /.medium-4.columns -->

</div><!-- /.row -->

We have a sports car, a simple sedan, or an old time classic. Another examples would be food:

<div class="row">
    <div class="medium-4 columns t30">
    <img src="{{ site.urlimg }}snacks.jpeg" alt="">
    </div><!-- /.medium-4.columns -->

    <div class="medium-4 columns t30">
      <img src="{{ site.urlimg }}entree.jpeg" alt="">
    </div><!-- /.medium-4.columns -->

    <div class="medium-4 columns t30">
      <img src="{{ site.urlimg }}dessert.jpeg" alt="">
    </div><!-- /.medium-4.columns -->

</div><!-- /.row -->

We have snacks, entrees, or desserts just to name a few of the different possibilities!

With this idea in the back of your mind, lets look at an example. 

## Example: Animal Kingdom
We can divide them into a few different groups:
* Mammals
* Birds
* Fish
* Reptiles
* Amphibians

Within each of these groups, we see animals that share similar characteristics. For instance, in the mammal group, we have dogs and wolves. Though different, they can both eat meat and howl. 
​
For each of those groups, think of them as ​objects. So the mammal group can be a single *object*. In that specific object, we can have actions like "noise" or "eat".

~~~
class Dog {
    public Dog() {}
    public void noise() {
        System.out.println("Bark! Bark!");
    }
    public void eat() {
        System.out.println("Eats dog food.");
    }	 
}
~~~

This dog object has the two functions, noise and eat. These are specific to this object. Therefore, suppose we did:

~~~ 
    Dog pug = new Dog();
    pug.noise();
~~~

We would have our pug say *Bark! Bark!* This is in essence what an object is, a class with different functions and attributes that this object can do and have. 

​Suppose now we want to make a dog. Since a dog is a mammal, we can create a dog object and pull actions from the mammal object such as "eat" since they share that attribute. That mammal object allowed us to *inherit* from that mammal instead of creating a whole other object. We can do the same with when creating a Wolf object too. 

We reduce the amount of work we have and code that we have to write by harnessing the power of OOP. We don't have to re-write the code for "eat" because our mammal object already has it.

To showcase the difference, let's examine the code below. The top is creating this mammal object and then creating a dog object. The second is creating the mammal object and then a brand new dog object.

~~~
abstract class Mammal {
    // abstract methods
    abstract void noise();
    abstract void eat();
}

class Dog extends Mammal {
    void noise() {
        System.out.println("Bark! Bark!");
    }
    void eat() {
        System.out.println("Eats dog food.");
    }	 
}

class Wolf extends Mammal {
    void noise() {
        System.out.println("Oowhoo");
    }
    void eat() {
        System.out.println("Eats sheep.");
    }
}
~~~

Above, we can see how Dog and Wolf both were able to reuse the same methods and adapt it. If we look below, we can see how slightly inefficient it would be if we didn't use objects and inherit.

~~~
class Dog {
    public Dog() {}
    public void noise() {
        System.out.println("Bark! Bark!");
    }
    public void eat() {
        System.out.println("Eats dog food.");
    }	 
}

class Wolf  {
    public Wolf() {}
    public void noise() {
        System.out.println("Oowhoo");
    }
    public void eat() {
        System.out.println("Eats sheep.");
    }
}
~~~

The difference is minute but becomes a larger problem when dealing will a plethora of objects. The difference is how we have to initialize a constructor for each object we are working with. 

