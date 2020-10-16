# JavaInterview

Q) Why is the Java main method static?
Ans) It is because the object is not required to call a static method. If it were a non-static method, JVM creates an object first then call main() method that will lead the problem of extra memory allocation.
Q) Can we execute a program without main() method?
Ans) No, one of the ways was the static block, but it was possible till JDK 1.6. Since JDK 1.7, it is not possible to execute a Java class without the main method.
Q) Call to this() mush be the first statement in constructor.
Ans)Compile Time Error: Call to this must be first statement in constructor

Q) Why multiple inheritance is not supported in java?
Ans) To reduce the complexity and simplify the language, multiple inheritance is not supported in java. Consider a scenario where A, B, and C are three classes. The C class inherits A and B classes. If A and B classes have the same method and you call it from child class object, there will be ambiguity to call the method of A or B class.

Q) Why Method Overloading is not possible by changing the return type of method only?
In java, method overloading is not possible by changing the return type of the method only because of ambiguity.
Compile Time Error: method add(int, int) is already defined in class Adder
Note: Compile Time Error is better than Run Time Error. So, java compiler renders compiler time error if you declare the same method having same parameters.
Q) Can we overload java main() method?
Ans) Yes, by method overloading. You can have any number of main methods in a class by method overloading. But JVM calls main() method which receives string array as arguments only.






Can we override static method?
No, a static method cannot be overridden. It can be proved by runtime polymorphism, so we will learn it later.

Why can we not override static method?
It is because the static method is bound with class whereas instance method is bound with an object. Static belongs to the class area, and an instance belongs to the heap area.

Can we override java main method?
No, because the main is a static method.

Q) Is final method inherited?
Ans) Yes, final method is inherited but you cannot override it. 
Q) What is blank or uninitialized final variable?
A final variable that is not initialized at the time of declaration is known as blank final variable.
Q) Can we initialize blank final variable?
Yes, but only in constructor.
Q) Can we declare a constructor final?
No, because constructor is never inherited.
Java Runtime Polymorphism with Data Member
Rule: Runtime polymorphism can't be achieved by data members.








