## .NET Framework

#### Q1. What is the difference between a stack and queue?
- [x] Stacks process value types by a top-down hierarchy - last in, first-out (LIFO). Queues follow this principle and insert items from the lower end while deleting ones from the top - first in, first-out (FIFO)


#### Q2. Which group contains all official types of JIT compilations?
- [x] Pre-JIT, Econo-JIT, Normal-JIT

#### Q3. What is Kestrel?
- [x] a cross-platform web server ASP.NET Core that is included by default in ASP.NET Core project templates\*\*

#### Q4. When would you use asynchronous actions?
- [x] to avoid blocking the request thread while waits for an I/O operation

#### Q5. What is CoreCLR?
- [x] CoreCLR is the .NET execution engine in .NET Core that performs functions like garbage collection and compilation to machine code.

#### Q6. When you define an abstract method, how do you use it in a derived class
- [x] In your derived class, override the method.

#### Q7. Which code do you use if you want to trigger a garbage collection in .NET?
- [x] `System.GC.Collect();`

#### Q8. You want to include language elements in a program. Which design pattern best fits this objective?
- [x] Interpreter <= correct

#### Q9. What makes a strong-named assembly?
- [x] a signed assembly

#### Q10. What happens when you concatenate two strings?
- [x] A third string object is created containing the concatenated strings.

#### Q11. What is a delegate?
- [x] A delegate in .NET is similar to a function pointer in C or C++. Using a delegate allows the programmer to encapsulate a reference to a method inside a delegate object.

#### Q12. Which is a set of features that extends the query capabilities of the .NET language syntax by adding sets of new standard query operators that allow data manipulation, regardless of the data source?
- [x] LINQ


#### Q13. What is the single responsibility principle?
- [x] A class should have only a single responsibility - that is, only changes to one part of the software's specification should be able to affect the specification of the class.

#### Q14. When should a developer use the .NET Standard class library project type?
- [x] when you want to increase the number of apps that are compatible with your library, and decrease the .NET API surface area your library can access

#### Q15. What is the difference between a SDK (software development kit) and runtime in .NET Core?
- [x] The runtime is the virtual machine that hosts and runs the application and abstracts all the interaction with the operating system; the SDK usually includes documentation and other help files.

#### Q16. What is the Common Type System (CTS)?
- [x] the component of CLI in which .NET Framework provides support for several languages since it contains a type system that is common with all the languages

#### Q17. Assuming y is a value type, which is an example of boxing?
- [x] object thisObject = y;

#### Q18. What is an abstract class in .NET?
- [x] An abstract class provides a partial implementation for functionality and some abstract or virtual members that must be implemented by the 

#### Q19. What is the namespace for caching information in .NET?
- [x] System.Runtime.Caching;

#### Q20. What is an interface in .NET?
- [x] An interface declares a contract or behavior that implementing classes require. It may declare only properties, methods, and events with no access modifiers. All the declared members must be implemented.

#### Q21. What does CAS stand for and what does it do?
- [x] CAS stands for Code Access Security and it enables users to restrict, on a very granular level, what managed code can do according to a level of trust.

#### Q22. Which is NOT true about lambda statements?
- [x] A statement lambda cannot return a value.

#### Q23. Which is NOT true about a read-only variable?
- [x] It can be initialized at declaration only.

#### Q24. What is the difference between System.String and string?
- [x] There is none—string is an alias for System. String.

#### Q25. When break is used inside two nested for loops, does control come out of the inner for loop or the outer for loop?
- [x] It breaks from only the inner loop.

#### Q26. You want to separate object construction from its representation. Which design pattern best fits this objective?
- [x] Builder

#### Q27. You want to encapsulate a command request as an object. Which design pattern best fits this objective?
- [x] Command


#### Q28. Why would Pre-JIT be used by the .NET Framework?
- [x] to compile complete source code into native code in a single compilation cycle during deployment of the application

#### Q29. What do code contracts do?
- [x] Code contracts provide a way to specify preconditions, postconditions, and object invariants in your code.

#### Q30. You must connect an app to an online identity provider using OAuth. For authentication, the app uses WebAuthenticationBroker object. You need to make sure the app registers with the provider. Which action do you take?
- [x] Invoke the AuthenticateAsync method and construct an HTTPS request URI.


#### Q31. You want to create a class of which only a single instance can exist. Which design pattern best fits this objective?
- [x] Singleton

#### Q32. What is the dependency inversion principle?
- [x] Entities must depend on abstractions, not on concrete implementations.

#### Q33. What is a namespace?
- [x] a group of classes, structures, interfaces, enumerations, and delegates—organized in a logical hierarchy by function that enable you to access the core functionality you need in your applications

#### Q34. Which of the following selects an anonymous type?
- [x] select new { a.Country, a.Region }


#### Q35. Which is NOT true about a constant variable?
- [x] At runtime, its value is evaluated.

#### Q36. What is the purpose of CLR?
- [x] CLR performs various operations such as memory management, security checks, assembly loading, and thread management. It also provides a secure execution environment for applications.

#### Q37. What is CIL?
- [x] Formerly known as MSIL, CIL is a programming language that NET developers use. It represents the lowest possible level for a language that humans can still read.

#### Q38. **\_** pattern works as a bridge between two incompatible interfaces? // wording in question is maybe changed?
- [x] Adapter

#### Q39. Why would you use ahead-of-time (AOT) compilation?
- [x] You can deliver a faster startup time, especially in big applications where much code executes on startup.

#### Q40. Which statement describes a Dispose method?
- [x] It belongs to the IDisposable interface and is used to free resources, such as network connection and files.

#### Q41. What is a thread?
- [x] A single operation that does not return a value and that usually executes asynchronously

#### Q42. You want to add responsibilities to object dynamically. Which design pattern best fit this objective?
- [x] Decorator

#### Q43. Which choice creates an 8-tuple containing prime numbers that are less than 20?
- [x] `var primes = Tuple.Create(2, 3, 5, 7, 11, 13, 17, 19);`

#### Q44. How can you recieve form data without a model binder in a controller action?
- [x] public IActionResult ReceivedDataByRequest()
      {
      string theName = Request.Form["theName"];
      return View();
      }

#### Q45. Where should you store connection string information?
- [x] in configuration files

#### Q46. Why use design patterns?
- [x] design patterns help you solve issues related to sofware development using a proven solution, and make communication between developers more efficient

#### Q47. What is a task?
- [x] a single operation that does not return a value and that usually executes asynchronously

#### Q48. Which choice is NOT a component of .NET Framework?
- [x] .NET framework class library

#### Q49. Which statement about the `this` keyword is _not_ true?
- [x] A constructor can use a base statement and a `this` statement if the base statement comes first.

#### Q50. When should you use the .NET Core class library project type?
- [x] when you want to increase the .NET API surface area your library can access, and allow only .NET Core apps to be compatible with your library


#### Q51. Why would the .NET Framework use Normal-JIT (Just-in-Time)?
- [x] to compile only methods called at runtime – which are compiled the first time the methods are called and then stored in a cache to be used for execution when the same methods are called again

#### Q52. What is .NET?
- [x] .NET is a free, cross-platform, open-source developer platform for building many different types of applications with multiple languages, editors, and libraries for web, mobile, desktop, gaming, and IoT.

#### Q53. The ASP.NET Core Module is a native IIS module that plugs into the IIS pipeline to either **\_**.
- [x] host an ASP.NET Code app inside of the IIS workes process, called the in-process hosting model, or forward web requests to a backend ASP.NET Core app running the Kestrel server, called the out-of-process hosting model

#### Q54. In the code below, what is the difference between RenderPartial and RenderAction?

```cs
@{
  Html.RenderAction("Add");
  Html.RenderPartial("Add");
}
```
- [x] RenderAction will call an action method of the current controller and render a result inline. RenderPartial will render the specified view inline without calling any action method.

#### Q55. What is the Liskov substitution principle?
- [x] Objects in a program should be replaceable with instances of their subtypes without altering the correctness of that program.

#### Q56. What method do you use to explicitly kill a user's session?
- [x] `Session.Abandon()`

#### Q57. Which choice best describes the difference between globalization and localization?
- [x] Globalization involves designing and developing a world-ready app that supports localized interfaces and regional data for users in multiple cultures. Localization is the process of translating an application's resources into versions for each culture that the application will support.

#### Q58. What does CIL stand for?
- [x] Common Intermediate Language

#### Q59. Which choice best describes the difference between a namespace and an assembly?
- [x] Namespace is the logical naming decided at design time by the developer. Scope for a particular type is defined at run time using an assembly.

#### Q60. What is a tuple?
- [x] A data structure that has a specific number and sequence of elements


#### Q61. What does IL stand for?
- [x] Intermediate Language


#### Q62. You want to create an instance of several families of classes. Which design pattern best fits this objective?
- [x] Abstract Factory


#### Q63. Which statement about a read-only variable is _not_ true?
- [x] It can be initialized at declaration only.

#### Q64. What is the interface segregation principle?
- [x] Many client-specific interfaces are better than one general-purpose interface.

#### Q65. Why would the .NET Framework use Econo-JIT (Just-inTime)?
- [x] to compile only the methods that are called at run time and remove them from memory after execution

#### Q66. What is the difference between a heap and a stack?
- [x] The stack contains stored value types; the heap contains stored reference types.


#### Q67. What is open closed principle?

- [x] software entities should be open for extension, but closed for modification.

#### Q68. How do you make sure that the garbage collector is done running when you call `GC.Collect()`?
- [x] by calling [`GC.WaitForFullGCComplete()`](https://docs.microsoft.com/en-us/dotnet/api/system.gc.waitforfullgccomplete)

#### Q69. What does JIT do in .Net?
- [x] JIT translates the IL code to an assembly code and uses the CPU architecture of the target machine to execute a .NET application.

#### Q70. Which statement about a constant variable is not `true`?
- [x] At run time, its value is evaluated.


#### Q71. What is the difference between managed and unmanaged code?
- [x] Managed code is code that is handled by the common language runtime (CLR). Unmanaged code is any code that does not depend on CLR for execution.

