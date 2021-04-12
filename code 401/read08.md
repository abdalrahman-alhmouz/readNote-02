#### SOLID :
![solid](https://static.javatpoint.com/core/images/solid-principles-java.png)
* SOLID is an acronym for the first five object-oriented design (OOD) principles by Robert C. Martin (also known as Uncle Bob).

##### Single-Responsibility Principle :
* A class should have one and only one reason to change, meaning that a class should have only one job.
* in real life :
* in your day to day life, picture those "duck" vehicles you see occasionally in some lakeside towns. they're street legal and water-capable, so a duck tour affords you the unique and surreal experience of being in a 'car' that gets to the edge of the water and just keeps going. fun, right?

and yet, you don't see a whole lot of them. there are millions of families out there that own both cars and boats, and there are very few families that buy these ducks. do you know why? it's most likely because no one wants to be unable to drive to work because their boat rudder is broken. ducks are fun, but they're also a great example of the pitfalls that the srp can help you avoid.


##### Open-Closed Principle :

* Objects or entities should be open for extension but closed for modification.
* in real life :
a great example of this in real life is sitting in your pocket in the form of a smartphone. all such phones have app stores and these app stores let you extend the base functionality of the phone. sure, it ships with the basics: camera operation, actual calls, text messages, etc. but via the app store, you can extend the phone's capabilities to allow you to manage your todo list, play inane video games, and even serve as a flashlight or wireless access point.

the mechanism that allows you to do this is purely one of extension, however. it's not as though apple, google, and microsoft put the os source code up on github and invite you to dive in and start building games and flashlight functionality. rather, they make the core phone functionality closed for modification and they open it to an extension .
##### Liskov Substitution Principle :

 * Let q(x) be a property provable about objects of x of type T. Then q(y) should be provable for objects y of type S where S is a subtype of T.
* in real life :
*  if you have a class, animal, with a makenoise() method, then any subclass of animal should reasonably implement makenoise(). cats should meow, dogs should bark, etc. what you wouldn't do is define a mutemouse class that throws idontactuallymakenoiseexception. this violates the lsp, and the argument would be that this class has no business inheriting from animal.

to picture this, imagine cooking yourself a stew. if you're anything like me, you'd only put things in there that were edible because you would want to eat the stew without picking through each bite, asking yourself repeatedly, "is this edible?"


##### Interface Segregation Principle :
* A client should never be forced to implement an interface that it doesn’t use, or clients shouldn’t be forced to depend on methods they do not use.
* in real life :
* the interface segregation principle (isp) says that you should favor many, smaller, client-specific interfaces over one larger, more monolithic interface. in short, you don't want to force clients to depend on things they don't actually need. imagine your code consuming some big, fat interface and having to re-compile/deploy with annoying frequency because some method you don't even care about got a new signature.

to picture this in the real world, think of going down to your local corner restaurant and checking out the menu. you'll see all of the normal menu mainstays, and then something that's just called "soup of the day." why do they do this? because the soup changes a lot and there's no sense reprinting the menus every day. clients that don't care about the soup needn't even be concerned, and clients that do use a different interface -- asking the server.

###### Dependency Inversion Principle :
Entities must depend on abstractions, not on concretions. It states that the high-level module must not depend on the low-level module, but they should depend on abstractions.
* in real life :
* the dependency inversion principle (dip) encourages you to write code that depends upon abstractions rather than upon concrete details. you can recognize this in the code you read by looking for a class or method that takes something generic like "stream" and performs operations on it, as opposed to instantiating a specific filestream or stringstream or whatever. this gives the code in question a lot more flexibility -- you can swap in anything that conforms to the stream abstraction and it will still work.

to visualize this in your day to day, go down to your local store and pay for something with a credit card. the clerk doesn't examine your card and get out the "visa machine" after seeing that your card is a visa. he just takes your card, whatever it is, and swipes it. both you and the clerk depend on the credit card abstraction without worrying about specifics.

