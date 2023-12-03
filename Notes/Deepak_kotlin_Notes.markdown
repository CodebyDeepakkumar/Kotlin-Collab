> This is my Kotlin Notes that I am learning from the Scaler course:\
> Kotlin is a JVM Language:\
> kotlin File (.kt) -\> (Compile) Byte Code -\> (Run) -\> JVM } Together
> a JDK Hello World Program :\
> fun main (args: Array\<string\>{ // main is the entry porint. args is
> the name of the parameter and Array\<string\> is the type of the
> parameter\
> println (\"Hello, World\")\
> }\
> Variables and Data Types:\
> var and val:\
> var: it can be reassigned\
> val: it cannot be reassigned(Like constant)
>
> var name = \'deepak\'\
> name = \'shivam\' // this will change\
> but,\
> val name = \'deepak\'\
> name = \'new\' // this won\'t be able to do it because of val\
> Data Types:\
> Integer, Floating, Boolean, Character(Chat, String)\
> We have an option to assign data type, else it is smart to understand
> the data type. then we can do:\
> var marks: Int = 24 //expilictly doing although not required
>
> Benefits:\
> Null safe, no null pointer exception.
>
> no need to add semicolon\
> ++a this will do the change first\
> a++ = a + 1 this is increameted post\
> classes and objects in Kotlin:
>
> Kotlin is an OOP language:\
> class is a blueprint for an object, house is the object one class can
> have multiple objects
>
> How to define classes:\
> //keyword called class\
> class ClassName {\
> //property\
> //member function\
> }
>
> //second example\
> Class lamp{\
> //property (data member)\
> Private var isOn: Boolean = false\
> //member function\
> Fun turnOn(){\
> isOn = true\
> }\
> //member function\
> Fun turnOff(){\
> isOn = false\
> }\
> }
>
> We have two member function turnOn () and turnOff()\
> Visibility modifiers:\
> Private - visible (can be accessed from inside the class only.
>
> Public - visible everywhere\
> Protected - visible to the class and its subclass\
> Internal - any client inside the module can access them.
>
> If we don't define the visibility modifier, it will be public by
> default
>
> Kotlin Objects
>
> No memory is created for the object\
> Val SampleObject = className() // new object is created.
>
> We access data members and data functions using dot : Fun main(){\
> Var obj1 = Person(name"Deepak", age: 25)\
> Obj.canVote(age:22)\
> }\
> sampleObject.isOn()

We can also create data members inside the constructor or see in the
example:

> class Person(var name: String, var age: Int){\
> Fun canVote(age: int){\
> if(age\<18){println("cannot vote")}\
> Else{println("Can Vote")}
>
> }\
> }
>
> Constructors :
>
> Concise way to initialise class properties\
> Special member function that is called when the object is created or
> instantiated.
>
> In kotlin:\
> primary constructor: concise way to initialize class\
> It is part of the class header it self: class Person(val name: String,
> var age: Int) Here val name will be read only propertycuz of val and
> var are of read-write property as it is declared with keyword.
>
> Secondary constructor: allows to put additional initialisation logic
> Init{ firstName = fName.capitalize()\
> Age = personAge\
> Println ("firstName = \$firstName")\
> println("Age = \$age")}
>
> ![](screenshots/media/image1.png){width="5.458333333333333in"
> height="5.020833333333333in"}
>
> In kotlin, we can create more than one secondary constructors. They
> are created using constructor keyword:

![](screenshots/media/image2.png){width="6.138888888888889in"
height="2.6041666666666665in"}

> How to extend classes:\
> To access the data member from the derived class, we use super
> keyword. As shown in the example below
>
> ![](screenshots/media/image3.png){width="5.458333333333333in"
> height="2.986111111111111in"}
>
> Kotlin Getters and Setters:\
> In kotlin, getters are to get value of the property and setters are to
> set the values of the property.
>
> in kotlin, they are auto generated and are optional.
>
> Lateinit: late initialisation.
>
> Such that I can initialise lateran in the program.
>
> As we can see in the below example, as I don't know about the
> profession, I will just initialise it with latinit keyword:
>
> ![](screenshots/media/image4.png){width="5.458333333333333in"
> height="4.348610017497813in"}
>
> Kotlin inheritance:

![](screenshots/media/image5.png){width="6.138888888888889in"
height="3.366665573053368in"}

> ![](screenshots/media/image6.png){width="5.458333333333333in"
> height="4.613888888888889in"}
>
> Kotlin searches for the init block (base class) in the class, so it
> will execute that class first
>
> Summary: If the class has a primary constructor, the base must be
> initialised using the parameters for the primary constructor. In the
> above program, both derived classes have two parameters age and name,
> and both these\
> parameters are initialised in primary constructor in the base class.
>
> Kotlin Visibility modifiers:
>
> It is used to modify the accessibility of classes, objects, interface,
> constructors, functions, properties and their setters. Getters take
> the visibility of the\
> property.

![](screenshots/media/image7.png){width="6.138888888888889in"
height="2.936111111111111in"}

> Note: If we override a protected member in the derived class without
> specifying its visibility, then its visibility will also be protected.
>
> Control Flow:
>
> If and Else:
>
> same as everywhere.
>
> When there are multiple cascading, then we use when () keyword.
>
> when(amber){\
> 0 -\> print("o")\
> 1 -\> print ("1")\
> Else -\> print("-1")\
> }\
> Like switch
>
> For Loop:
>
> Iterate through a range:\
> fun main(args: Array\<string\>){\
> For (I in 1..5)}{\
> println(I)\
> }\
> }
>
> Output:\
> 1\
> 2\
> 3\
> 4
>
> 5\
> Iterating through a string:\
> Fun main(args:Array\<String\>){\
> Var text = 'kotlin'\
> For (letter in text ) {\
> Print ln(letter)\
> }
>
> }
>
> Output:
>
> K\
> o\
> t\
> l\
> i\
> n
