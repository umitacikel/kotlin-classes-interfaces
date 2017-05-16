# kotlin-classes-interfaces

Classes:

Classes in Kotlin are declared using the keyword Class. Classes in Kotlin can contain Constructors and initializer blocks Functions Properties Nested and Inner Classes Object Declarations Constructors: There is two types of constructors in Kotlin(Primary, secondary) The primary constructor is a part of the header

class Person constructor(firstName: String) { 

}

but, you can be typed in this way

class Person(firstName: String) { 

}

secondary constructor is a child of the primary

class Person(val name: String) { constructor(name: String, parent: Person) : this(name) { parent.children.add(this) } }

Interfaces:

Interfaces in Kotlin are very similar to Java 8. They can contain declarations of abstract methods, as well as method implementations. What makes them different from abstract classes is that interfaces cannot store state. They can have properties but these need to be abstract or to provide accessor implementations.

An interface is defined using the keyword interface

interface MyInterface { 
    fun bar() 
    fun foo() { 
    } 
   }
