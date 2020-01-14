# Object-Oriented Programming Concepts

Alan Curtis Kay is widely considered one of the fathers of object-oriented programming, which he named, along with some colleagues, at the Palo Alto Research Center (PARC), formerly known as Xerox PARC.

  > The fundamental difference between structured programming and object-oriented programming can be  summarized as follows: In object-oriented programming, instead of focusing on the operations on data, focus on the data itself.

## Class and Objects

These are at the core of OOP. A class is the blueprint or template for its objects. Objects are instances of a class. Each object has its own state, behavior, and identity. In simple language, you can say that in structured programming, you segregate the problem into small functions, and in OOP, you divide the problem into objects. You are familiar with data types like int, double, float, and so forth. You know that these are built-in data types or primitive data types because they are already defined in a computer language. But when you create your own data type, let’s say, Student, you need to create a Student class. Just as when you need to create an integer variable, you mention the int first, similarly, when you need to create a Student object (e.g., john), you need to mention your Student class first. So, when you’re familiar with OOP, you may say something like this: a dog is an object from a Mammal class, your car is an object from a Vehicle class, and so on.

## Encapsulation

In object-oriented programming, you do not allow your data to flow freely inside the system. Instead, you wrap the data and functions into a single unit (i.e., in a class). The purpose of encapsulation is at least one of the following:
  *  Putting restrictions in place so that the components of an object cannot be accessed directly
  *  Binding the data with methods that will act on that data (i.e., forming a capsule)

In some OOP languages, the hiding of the information is not implemented by default. So, they come up with an additional term called *information hiding*.

Later, you will see that data encapsulation is one of the key features in a class. If you want to promote security, your data should not be visible to the outside world. Only through the methods defined inside the class can you access these data. Therefore, you can think of these methods as the interface between the objects’ data and the outside world (i.e., your program). In Java, you can implement encapsulation in various ways. For example, you can use the access specifiers (or modifiers) and getter-setter methods in this context

## Abstraction

The key purpose of abstraction is to show only the essential features and to hide the background details of implementation. Abstraction is also very much related to encapsulation, but the difference may be easily understood with a simple day-to-day scenario.

When you press a button on your remote control to switch on the TV, you do not care about the internal circuits of the TV or how the remote control controls the operation of the TV. You simply know that different buttons on the remote control have different functionalities, and as long as they work properly, you are happy. So, the user is isolated from the complex implementation details, which are encapsulated within the remote control (and TV). At the same time, the common operations that can be performed through the remote control can be thought of as an abstraction. A manufacturer can enhance this feature when the same remote can also perform on a different model or product. For example, a DVD player’s remote control can also be used to control the volume of a TV.

## Inheritance

Whenever we talk about reusability, we’ll generally refer to inheritance, which is a process in which one object acquires the properties of another object. Consider this example. `Bus` is one type of `Vehicle` because it fulfills the basic criteria of a `Vehicle` that is used for transportation purposes. Similarly, `Train` is another type of `Vehicle`. And even though a `GoodsTrain` and a `PassengerTrain` are different, we can say that both inherit from the `Train` category (or class) because ultimately both of them fulfill the basic criteria of a `Train`, which in turn is a `Vehicle`. So, you can simply say that hierarchical classifications are supported with the concept of inheritance.

In the programming world, inheritance creates a new child class from an existing parent class. This parent class is sometimes known by different names. For example, in C#, you call this parent class the base class and in Java, you may refer to it as the super class. So, in simple words, a parent class is placed one level up in that hierarchical chain. Then you can add new functionalities (methods) or modify the super class functionalities (later you will call it overriding the functionalities) into the child class. You must remember that due to these modifications, the core architecture should not be affected. In other words, if you derive `Bus` class from `Vehicle` class, and add/modify the functionalities in `Bus` class, those modifications will not impact the original functionalities that were described for the `Vehicle` class.

So, the key advantage is that you can avoid lots of duplicate code with this mechanism.

## Polymorphism

Polymorphism is generally associated with one name with many forms. Consider the behavior of your pet dog. When it sees an unknown person, it is angry and starts barking a lot. But when it sees you, it makes different noises and behaves differently. In the coding world, you can also think of a common method, addition. With addition in the context of two integers, you expect to get a sum of the integers. But for string operands, you expect to get a concatenated string.

*Polymorphism* can be of two types:

  * **Compile-time polymorphism**: The compiler can decide very early which method to invoke in which situation once the program is compiled. This is also known as static binding or early binding.
  * **Runtime polymorphism**: The actual method calls are resolved at runtime. At compile time, you cannot predict which method will be invoked when the program runs (for example, the program may behave differently with different inputs). Consider the following case: suppose you want to generate a random number at the very first line when you execute a program. If the generated number is an even number, you will call a method, Method1(), which prints “Hello”; otherwise, you’ll call a method whose name is the same but prints “Hi.” Now, you’ll agree that after you execute the program, you can only see which method is invoked (i.e., the compiler cannot resolve the call at compile time). In a situation like this, you do not have any clue as to whether you will see “Hello” or “Hi” prior to the program’s execution. Therefore, sometimes it is also termed dynamic binding or late binding.

# Q&A Session

1. What are the key features of object-oriented programming?
> The following are the key features of object-oriented programming:
    >* Encapsulation
    >* Abstraction
    >* Inheritance
    >* Polymorphism

2. How is an object different from a class?
> Objects are made from a class. An object is an instance of a class, which is just a template or a blueprint for your object. An object is a physical entity and can allocate memory in the system, but class is a logical entity and does not allocate memory in the system.

3. How is abstraction different from encapsulation?
> Abstraction focuses on the noticeable behavior of an object, and encapsulation focuses on the implementation part of that behavior. Encapsulation helps you to bundle your data, and at the same time it can hide some information that you do not want to disclose to the outside world.

4. What is the key advantage associated with the inheritance mechanism?

> Reusing the existing code, you can save time and effort. At the same time, this mechanism helps you to avoid duplicate codes in your application.

5. What are the characteristics of object-oriented programming?
> Here are some important characteristics:
>  * Your focus is on data, not on functions. So, you divide your program into objects, not functions.
>  * You do not allow data to flow freely. You use methods to access them.
>  * Your objects communicate through methods.
>  * The outside world should not access your data.
>  * Your application can adapt to new changes easily. At the same time, it is easy to maintain.