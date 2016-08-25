# Homework

Today we looked at the Strategy and Template pattern. There are many other patterns that developers have come up with that we can also use.

Choose one or more of the following patterns to investigate:

- Singleton 
- Factory
- State
- Command
- Decorator
- Facade
- Observer
- Chain of Responsibility

Create an example and write an explanation of it in your own words.

You can find good examples here: 
http://www.tutorialspoint.com/design_pattern/

Singleton Pattern

How to create one-of-a-kind objects for which there is only one instance.
Simplest pattern in terms of its class diagram, as it just holds a single class.

It’s a convention for ensuring one and only one object is instantiated for a given class. 
Downside:
Singleton code is hard to get right - how do you prevent more than one object being instantiated?

If you have an object that contains registry settings, you don’t want multiple copies of that object and its values around - that would be chaos.
By using a singleton pattern, you can assure that every object in your application is making use of the same global resource.

Many developers run into bugs because they have multiple copies of objects floating around that they’re not even aware of.

They have no public constructor - it is declared private.
So in order to get a hold of a Singleton object, you don’t instantiate it, you just ask for an instance of it.

So the class has a static method called getInstance()
If you call that, the object will show up at once.

The Singleton Pattern ensures a class has only one instance, and provides a global point of access to it.

We’re taking a class and letting it manage a single instance of itself. We’re also preventing any other class from creating a new instance on its own.
To get an instance, you have to go through the class itself.

So whenever you need an instance, just query the class and it will hand you back the single instance.

Example:

public class SingleObject
create an object
make the constructor private so that it cannot be instantiated
Get the only object 
