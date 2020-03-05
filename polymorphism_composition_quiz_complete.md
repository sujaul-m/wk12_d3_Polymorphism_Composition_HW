# Polymorphism & Composition Homework - Quiz

# Polymorphism

1. What does the ___word___ 'polymorphism' mean?
Answer - Polymorphism means "many forms"

2. What does it mean when we apply polymorphism to OO design? Give a simple Java example.
Answer - it means we are treating an instance of a class as if it is another class or type at the same time.

```java
public interface IVehicle{}
public class Car implements IVehicle{}

Car car = new Car();
IVehicle vehicle = car;
```

3. What can we use to implement polymorphism in Java?
Answer - we can make use of inheritance, abstract classes and interfaces.

4. How many 'forms' can an object take when using polymorphism?
Answer - an object can take as many forms as it needs.

5. Give an example of when you could use polymorphism.
Answer - You would use polymorphism if you wanted a class to have a collection of different types of objects and be able to add objects of those types to the collection e.g:

```java
public interface IFood{}
public class Zebra implements IFood{}
public class Deer implements IFood{}

public class Lion() {
  ArrayList<IFood> belly;

  public Lion() {
    belly = new ArrayList<IFood>();
  }

  public void eat(IFood food) {
    belly.add(food)
  }
}

Lion lion = new Lion();
IFood zebra = new Zebra();
IFood deer = new Deer();

lion.eat(zebra);
lion.eat(deer);
```

# Composition

6. What do we mean by 'composition' in reference to object-oriented programming?
Answer - It describes a class that references one or more objects of other classes in instance variables

7. When would you use composition? Provide a simple example in Java.
Answer - You would use composition when you want to model an object that will have other objects, rather than inheriting from them

8. What is/are the advantage(s) of using composition?
Answer - It is much more flexible than inheritance.

9. When an object is destroyed, what happens to all the objects it is composed of?
Answer - They are all Destroyed
