# Packages and Import
* A package in Java is used to group related classes. Think of it as a folder in a file directory. We use packages to avoid name conflicts, and to write a better maintainable code. 
![package](https://simplesnippets.tech/wp-content/uploads/2018/04/packages-in-java-programming-featured-image-1280x720.jpg)
* The first statement, other than comments, in a Java source file, must be the package declaration.

### Imports: three options
* The JOptionPane class is in the swing package, which is located in the javax package. The wildcard character (*) is used to specify that all classes with that package are available to your program. This is the most common programming style.

###### import FAQ
Q: Does importing all classes in a package make my object file (.class or .jar) larger?
 * A: No, import only tells the compiler where to look for symbols.

Q: Is it less efficient to import all classes than only the classes I need?
 * A: No. The search for names is very efficient so there is no effective difference.

Q: Doesn't it provide better documentation to import each class explicitly?
 * A: This shows good intentions, but ...

 * It's hard to remember to remove classes when they are no longer used, so the import list is surprisingly often wrong. It can seriously slow down reading because unusual or unexpected class imports make me look for that class, only to discover that it must have been used in an earlier version.
Explicit class imports permit accidentally defining classes with names that conflict with the standard library names. This is very bad. Using "*" to import all classes prevents this dangerous naming accident.
It's annoying to always update this list, altho if you use NetBeans, fixing the list is only a click away (see below).

### loop in java :

 ##### for loop :
 * A for loop is a control structure that allows us to repeat certain operations by incrementing and evaluating a loop counter.
 ##### While  loop :
 * The while loop is Java's most fundamental loop statement. It repeats a statement or a block of statements while its controlling Boolean-expression is true.

 :
 ##### Do-While Loop :
* The do-while loop works just like the while loop except for the fact that the first condition evaluation happens after the first iteration of the loop.

![loop](https://1.bp.blogspot.com/-mcTB2UoPY1E/WxtaTUjMXYI/AAAAAAAAAKc/zWqmuTOIzo06TLhKFL9cXLRqr_ymQ3mnACLcBGAs/s1600/types-of-loop-in-java.png)
