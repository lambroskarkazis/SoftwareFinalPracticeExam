# RAIK 383H: Software Engineering Practice Final Solutions
#### Spring 2017
#### Professor Mihaela Bobaru
#### Author Lambros Karkazis

### Question 1

Our group took a number of steps to manage complexity.

1. We used Github as source control.
2. We implemented the .NET MVC architecture.
3. We used Visual Studio's IntelliSense.

#### Github
Source control enabled the team to effectively collaborate. If a problem occurred git enabled us to pinpoint which changes caused the problem. Further, it ensured that different collaborators did not interfere with one another while developing. Oftentimes, no merge conflicts occurred.  

#### .NET MVC
Our choice of framework eased complexity. The framework has great documentation. Many have used it, so we could avoid other's mistakes. The MVC architecture adequately separates the project's parts.

#### Visual Studio
Visual Studio manages complexity with code highlighting and IntelliSense. By presenting software well, the programmer can better manage the codebase. IntelliSense allows programmers to understand the context of a code snippet. Further, it directly indicates when a developer makes incorrect assumptions.  

### Question 2

Agile welcomes change. With that in mind, Agile fits projects that require large amounts of change.  For example, if a customer does not know exactly what kind of software it needs, Agile will help it find a good solution.Importantly, Agile needs an active client to interact with the project manager. If the client does not want to interact with the development team, Agile will not function properly.

On the other hand, some software projects have well-defined specifications from the start. Many security specific applications require thorough specifications prior to development. Furthermore, embedded systems often have well defined specs since each modular component needs to interact in a well-defined manner.  

### Question 3

Component-level testing ensures that processes work together properly. In this case, we want a component test that ensures that the FinishSemester and AddCourse functions work properly in this program. A component-test that could ensure that these two work properly together. For example, try running FinishSemester then begin adding courses.

Looking at the code, a number of issues could occur. For one thing, FinishSemester does not clear the currentCourses. This would cause problems if another function did not properly clear the currentCourses. This code could also cause concurrency problems. Usually, students try to enroll in courses before the end of a semester. This code could cause problems if students seem to get added to courses that they do not actually take.

### Question 4

Data modeling allows programmers to decide what information the program will deal with and how that information gets organized. Since all computing tasks deal with information (and the manipulation of information), deciding what information falls in the domain of a problem defines how the team will solve the problem.

### Question 5

Pretend that you develop software for a banking company. You need to write code for a new ATM. For this project, the ability to take input from a keypad is a functional requirement. The project needs this to work for the project to succeed. On the other hand, _timely_ keyboard input is a non-functional requirement. Users expect responsive applications. Since this requirement depends on user's perception of functionality rather than actual functionality, it is a non-functional requirement.

### Question 6

High cohesion means that multiple components `play well' with each other. Loose coupling means that individual components do not depend heavily on one another. Applying these concepts to software products results in better code. If a software project has highly cohesive parts, it will result in fewer pieces and fewer lines of code. When each interaction between software pieces yields meaningful results, the software projects need less pieces and less interactions. When software projects have loosely coupled parts, the project has less complexity. A change in one piece does not cause the entire system to break.

