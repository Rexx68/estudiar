## C#

#### Q1. In which of these situations are interfaces better than abstract classes?

- [x] When you need a list of capabilities and data that are classes-agnostic, use an interface. When you need a certain object type to share characteristics, use an abstract class.


#### Q2. Which statement is true of delegates?

- [x] They can be chained together.

[Official documentation: Delegates](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/delegates/#delegates-overview)

#### Q3. Which choice best defines C#'s asynchronous programming model?

- [x] task-based

[Official documentation: Task asynchronous programming model](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/concepts/async/task-asynchronous-programming-model)

resposta correta --> var contacts = new List<string>();

#### Q4. How would you determine if a class has a particular attribute?

- [x] .

```cs
Attribute.GetCustomAttribute(typeof(ExampleController), typeof(SubControllerActionToViewDataAttribute))
```

[Official documentation: Attribute Class](https://docs.microsoft.com/en-us/dotnet/api/system.attribute?view=net-5.0)

[Official documentation: Attribute.GetCustomAttribute Method](https://docs.microsoft.com/en-us/dotnet/api/system.attribute.getcustomattribute?view=net-5.0)

#### Q5. What is the difference between the ref and out keywords?

- [x] Variables passed to out can be passed to a function without being initialized, while ref specifies that the value is a reference value that can be changed inside the calling method.

[Official documentation: ref](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/ref)

[Official documentation: out parameter modifier](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/out-parameter-modifier)

#### Q6. How could you retrieve information about a class, as well as create an instance at runtime?

- [x] reflection

[Official documentation: Reflection ](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/concepts/reflection)

#### Q7. What is this code an example of?

```cs
    private static object objA;
    private static object objB;

    private static void performTaskA()
    {
        lock (objB)
        {
            Thread.Sleep(1000);
            lock (objA) { }
        }
    }

    private static void PerformTaskB()
    {
        lock (objA)
        {
            lock (objB) { }
        }
    }
```

- [x] a potential deadlock

[Official documentation: Deadlocks and race conditions](https://docs.microsoft.com/en-us/dotnet/standard/threading/managed-threading-best-practices#deadlocks-and-race-conditions)

#### Q8. What is the difference between an anonymous type and a regular data type?

- [x] Anonymous types don't have type names

[Official documentation: Anonymous Types](https://docs.microsoft.com/en-us/dotnet/csharp/fundamentals/types/anonymous-types)

#### Q9. When would you use a Dictionary rather that an Array type in your application?

- [x] when you need to store key-value pairs rather than single values

[Official documentation: Dictionary<TKey,TValue> Class](https://docs.microsoft.com/en-us/dotnet/api/system.collections.generic.dictionary-2?view=net-5.0)

#### Q10. What is the difference between a.Equals(b) and a == b?

- [x] The .Equals method compares contents while `==` compares reference identity.

[Official documentation: Object.Equals](https://docs.microsoft.com/en-us/dotnet/api/system.object.equals)

[c-sharpcorner: Equality Operator(==) vs .Equals()](https://www.c-sharpcorner.com/UploadFile/3d39b4/difference-between-operator-and-equals-method-in-C-Sharp)

#### Q11. Which choice best describes a deadlock situation?

- [x] when simultaneous instructions are waiting on each other to finish before executing

[Official documentation: Deadlocks and race conditions](https://docs.microsoft.com/en-us/dotnet/standard/threading/managed-threading-best-practices#deadlocks-and-race-conditions)

#### Q12. How does the async keyword work?

- [x] It allows the await keyword to be used in a method

[Official documentation: async](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/async)

#### Q13. What is an object in C#?

- [x] an instance of a class or struct that includes fields, properties, and/or methods

[Official documentation: Objects](https://docs.microsoft.com/en-us/dotnet/csharp/fundamentals/object-oriented/objects)

#### Q14. Which code snippet declares an anonymous type named userData?

- [x] `var userData = new { name = "John", age = 32 };`

[Official documentation: Anonymous Types](https://docs.microsoft.com/en-us/dotnet/csharp/fundamentals/types/anonymous-types)

#### Q15. What will be returned when this method is executed?

`public void userInput(string charParameters) { }`

- [x] nothing

[Official documentation: void](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/void)

#### Q16. In what order would the employee names in this example be printed to the console?

```cs
string[] employees = { "Joe", "Bob", "Carol", "Alice", "Will" };

IEnumerable<string> employeeQuery = from person in employees
                                    orderby person
                                    select person;

foreach(string employee in employeeQuery)
{
    Console.WriteLine(employee);
}
```

- [x] ascending

[dotnetpattern: LINQ OrderBy Operator](http://dotnetpattern.com/linq-orderby-operator)

#### Q17. Lambda expressions are often used in tandem with which of the following?

- [x] LINQ

[Official documentation: Language Integrated Query (LINQ) Overview](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/concepts/linq/)

#### Q18. What is the correct formatting for single line and multiline comments?

      / Single Line
- [x] // Single Line
      /_ Multiline _/

[w3schools: C# Comments](https://www.w3schools.com/cs/cs_comments.php)

#### Q19. How do you make a method in an abstract class overridable?

- [x] Make it virtual

[Official documentation: virtual](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/virtual)

[Official documentation: abstract](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/abstract)

#### Q20. How would you write code for an integer property called Age with a getter and setter?

- [x] public int Age { get; set; }

[Official documentation: Using Properties](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/classes-and-structs/using-properties)

#### Q21. What is an abstract class?

- [x] a class that can be used only as base class

[Official documentation: Abstract and Sealed Classes and Class Members](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/classes-and-structs/abstract-and-sealed-classes-and-class-members)

#### Q22. When using a thread pool what happens to a given thread after it finishes its task?

- [x] The thread returns to the pool for reuse.

[Official documentation: Thread pool characteristics](https://docs.microsoft.com/en-us/dotnet/standard/threading/the-managed-thread-pool#thread-pool-characteristics)

#### Q23. Which choice represents a class that inherits behavior from a base class?

- [x] a derived class


[Official documentation: Inheritance](https://docs.microsoft.com/en-us/dotnet/csharp/fundamentals/object-oriented/inheritance)

#### Q24. What does operator overloading allow you to do?

- [x] define custom functionality for common operators like addition and equality

[Official documentation: Operator overloading](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/operators/operator-overloading)

#### Q25. What is the main purpose of LINQ?

- [x] to query and transform data


[Official documentation: Language Integrated Query (LINQ) Overview](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/concepts/linq/#query-expression-overview)

#### Q26. What is the correct syntax for a new generic list of strings named contacts?

- [x] var contacts = new List<string>();


[Official documentation: List<T> Class](https://docs.microsoft.com/en-us/dotnet/api/system.collections.generic.list-1?view=net-5.0)

#### Q27. What is the difference between throw exceptions and throw clauses?

- [x] Throw exceptions overwrite the stack trace, while throw clauses retain the stack information.


[Official documentation: throw](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/throw)

[c-sharpcorner: Difference Between Throw Exception and Throw Clause](https://www.c-sharpcorner.com/UploadFile/akkiraju/difference-between-throw-exception-and-throw-clause/)

#### Q28. When an asynchronous method is executed, the code runs but nothing happens other than a compiler warning. What is most likely causing the method to not return anything?

- [x] The method is missing an await keyword in its body.

[Official documentation: Starting tasks concurrently](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/concepts/async/#start-tasks-concurrently)

#### Q29. What are C# events?

- [x] actions that generate notifications, which are sent to their registered listeners

[Official documentation: Introduction to events](https://docs.microsoft.com/en-us/dotnet/csharp/events-overview)

#### Q30. What kind of values can arrays store?

- [x] multiple variables, or collections, of the same type

[Official documentation: Arrays](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/arrays/)

#### Q31. Given this enumeration, how would you access the integer-type value of 'AppState.Loading'?

`enum AppState { OffLine, Loading, Ready }`

- [x] int currentState = (int)AppState.Loading;

[Official documentation: Enumeration types](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/enum#conversions)

#### Q32. What character would you use to start a regular expression pattern at a word boundary?

- [x] \b

[regular-expressions: Word Boundaries](https://www.regular-expressions.info/wordboundaries.html)

[Official documentation: Regular Expression Language - Quick Reference](https://docs.microsoft.com/en-us/dotnet/standard/base-types/regular-expression-language-quick-reference)

#### Q33. To conform to the following interface, which of its members need to be implemented?

```cs
public interface INameable
{
    string FirstName { get; set; }
    string LastName { get; }
}
```

- [x] Both the FirstName and LastName properties need to be implemented.

[Official documentation: interface](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/interface)

#### Q34. You're dealing with multiple assemblies in your program, but are worried about memory allocation. At what point in the program life cycle are assemblies loaded into memory?

- [x] only when required

1. [Official documentation: Assembly Loading](https://docs.microsoft.com/en-us/dotnet/framework/deployment/best-practices-for-assembly-loading)
2. [Stackoverflow : When exactly are assemblies loaded?](https://stackoverflow.com/questions/21914692/when-exactly-are-assemblies-loaded)

#### Q35. What is most accurate description of a regular expression?

- [x] A regular expression is a special text string for describing a search patters.

1. [Official documentation: Regular Expression Language - Quick Reference](https://docs.microsoft.com/en-us/dotnet/standard/base-types/regular-expression-language-quick-reference)
2. [Official documentation: .NET regular expressions](https://docs.microsoft.com/en-us/dotnet/standard/base-types/regular-expressions)

#### Q36. Why would you use a class field in C#

- [x] To hold information and data contained in the class object

[Official documentation: Introduction to classes](https://docs.microsoft.com/en-us/dotnet/csharp/fundamentals/types/classes)

#### Q37. When would you use generics in your code?

- [x] all of these answers

[Official documentation: Generic classes and methods](https://docs.microsoft.com/en-us/dotnet/csharp/fundamentals/types/generics)

#### Q38. What prints to the console when this code is executed?

```cs
public delegate void AuthCallback(bool validUser);
public static AuthCallback loginCallback = Login;
public static void Login()
{
    Console.WriteLine("Valid user!");
}

public static void Main(string[] args)
{
    loginCallback(true);
}
```

- [x] an error, because the method signature of Login doesn't match the delegate

1. [Official documentation: Introduction to Delegates](https://docs.microsoft.com/en-us/dotnet/csharp/delegates-overview)
2. [Official documentation: Introduction to Events](https://docs.microsoft.com/en-us/dotnet/csharp/events-overview)

#### Q39. How would you declare a sealed class named User?

- [x] sealed class User {}


[Official documentation: Abstract and Sealed Classes and Class Members](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/classes-and-structs/abstract-and-sealed-classes-and-class-members)

#### Q40. What is the difference between non-static and static classes?

- [x] non-static classes need to be initialized before use, while static classes do not


1. [stackoverflow](https://stackoverflow.com/questions/20451554/whats-the-function-of-a-static-constructor-in-a-non-static-class)
2. [Official documentation: Static Constructors](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/classes-and-structs/static-constructors)

#### Q41. Which characteristic prevents this code from compiling?

`public int age="28"`

- [x] type safety

[c-sharpcorner: Type Safety in .NET](https://www.c-sharpcorner.com/UploadFile/vikie4u/type-safety-in-net/)

#### Q42. How would you serialize this class?

`public class User {}`

- [x] Mark the User class with the `SerializableAttribute` attribute.


[Official documentation: SerializableAttribute Class](https://docs.microsoft.com/en-us/dotnet/api/system.serializableattribute?view=net-5.0)

#### Q43. How would you write a delegate named ResultCallback with an int parameter named responseCode?

- [x] public delegate void ResultCallback(int responseCode);

[Official documentation: Delegates](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/delegates/)

#### Q44. What is the difference between a static and non-static method?

- [x] static methods do not have to instantiate an instance of the class to call the method

[Official documentation: Static Members](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/classes-and-structs/static-classes-and-static-class-members#static-members)

#### Q45. What is the correct way to write an event named apiResult based on a delegate named ResultCallback?

- [x] public event ResultCallback apiResult;

[Official documentation: Introduction to events](https://docs.microsoft.com/en-us/dotnet/csharp/events-overview)

#### Q46. When will the code inside finally block be executed in a try-catch statement?

- [x] after the try and catch blocks

[Official documentation: try-catch](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/try-catch)

#### Q47. What method correctly extends the string class?

- [x] public static string IsvalidName(this string i, string value) {}


#### Q48. How are C# classes limited?

- [x] They do not support multiple inheritance.

[Official documentation: Class inheritance](https://docs.microsoft.com/en-us/dotnet/csharp/fundamentals/types/classes#class-inheritance)

#### Q49. What function do namespaces perform?

- [x] Namespaces separate code into groupings, control access, and void naming collisions.

[Official documentation: namespace](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/namespace)

#### Q50. What is the correct way to write a public property with a private backing field?

- [x]

```cs
private int _password;
public int Password
{
  get { return _password; }
  set { _password = value; }
}
```

[Official documentation: Using Properties](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/classes-and-structs/using-properties)

#### Q51. What is a thread pool?

- [x] a collection of threads created during initialization that can be reused


[Official documentation: ThreadPool Class](https://docs.microsoft.com/en-us/dotnet/api/system.threading.threadpool?view=net-5.0)

#### Q52. When an object in C# is serialized, what is it converted to?

- [x] byte stream

[Official documentation: Serialization](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/concepts/serialization/)

#### Q53. What is a delegate

- [x] a type that holds a reference to a method with a particular parameter list and return type

[Official documentation: Delegates](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/delegates/)

#### Q54. What are the four keywords associated with exception handling in C#?

- [x] try, catch, finally, throw

[Tutorial Point](https://www.tutorialspoint.com/csharp/csharp_exception_handling.htm#:~:text=Exceptions%20provide%20a%20way%20to,catch%2C%20finally%2C%20and%20throw.)

#### Q55. What is the main difference between the is and as operators?

- [x] The is operator checks object type, while the as operator attempts to cast an object to a specific type.

[Pluralsight guide](https://www.pluralsight.com/guides/csharp-is-as-operators-is-expressions)

#### Q56. What is the difference between finally and finalize blocks?

- [x] The finally block is called after the execution of a try and catch block, while the finalize method is called just before garbage collection.

[C-sharpcorner](https://www.c-sharpcorner.com/forums/final-finally-and-finalize)

#### Q57. Your application has a value type called username that needs to be able to accept null values, but this is generating compile-time errors. How would you fix this in code?

- [x] string? username = null;


#### Q58. Which code snippet correctly declares a custom exception named InvalidResponse?

- [x] class InvalidResponse: Exception {}

[Official documentation: Exceptions](https://docs.microsoft.com/en-us/dotnet/standard/exceptions/how-to-create-user-defined-exceptions)

#### Q59. How would you write an enum variable called AppState with values for Offline, Loading, and Ready?

- [x] enum AppState {Offline, Loading, Ready}

[Official documentation: Enum](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/enum)

#### Q60. What is the main difference between a value type and a reference type?

- [x] A value type stores an actual value, while a reference type is a pointer to a value.

[Official documentation: Value types](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/value-types)

[Official documentation: Reference types](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/reference-types)

#### Q61. What is the difference between the `break` and `continue` keywords?

- [x] The `break` keyword literally breaks out of a control flow statement, while `continue` ignores the rest of the control statement or iteration and starts the next one.

[Official documentation: Jump statements](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/statements/jump-statements)

#### Q62. Which code snippet correctly declares a variable named userId with a public `get` and private `set`?

- [x] `public int userID { get; private set; }`

[Official documentation: Properties](https://docs.microsoft.com/en-us/dotnet/csharp/properties)

#### Q63. What is true about virtual methods?

- [x] `Virtual methods always need a default implementation.`

1. [Official documentation: virtual](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/virtual)
2. [c-sharpcorner: Virtual Method in C#](https://www.c-sharpcorner.com/UploadFile/3d39b4/virtual-method-in-C-Sharp/)

#### Q64. What is likely to happen if you have multiple threads accessing the same resource in your program?
    
- [x] `deadlock and race conditions`

[Official documentation: race conditions](https://docs.microsoft.com/en-us/archive/msdn-magazine/2008/october/concurrency-hazards-solving-problems-in-your-multithreaded-code)

#### Q65. How do you indicate that a string might be null?

- [x] `string? myVariable`

    
#### Q66. Do you need to declare an out variable before you use it?

- [x] `No, you can declare it in the parameter list.`


#### Q67. How would you access the last two people in an array named People?

- [x] `People[..^2]`

[Official Documentation: Ranges](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/proposals/csharp-8.0/ranges)

#### Q68. When can anonymous types be created?

- [x] `at compile time`

[C-sharpcorner: Anonymous Types](https://www.c-sharpcorner.com/UploadFile/ff2f08/anonymous-types-in-C-Sharp/)

#### Q69. What is true about thread multitasking?

- [x] `Thread multitasking allows code to be executed concurrently`

[Official Documentation: Threads](https://docs.microsoft.com/en-us/dotnet/standard/threading/threads-and-threading)

#### Q70. What accessibility level does this class field have ?

`private string LastName;`

- [x] It can be used by other code only in the same class or struct.

[Official Documentation: Accessibility Levels](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/accessibility-levels)

#### Q71. How would you correctly declare a jagged array called 'partyInvites' with 10 empty elements?

- [x] `string[][] partyInvites = new string[10][];`

[Official Documentation: Jagged Arrays](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/arrays/jagged-arrays)

#### Q72. How could you pause a thread for three seconds?

- [x] Thread.Sleep(3000);

[Official Documentation: https://docs.microsoft.com/en-us/dotnet/api/system.threading.thread.sleep?view=net-6.0]
