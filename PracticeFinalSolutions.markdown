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

### Question 7

Our choice of framework eased complexity. The framework has great documentation. Many have used it, so we could avoid other's mistakes. The MVC architecture adequately separates the project's parts. (Note: this part came right from an earlier question)

### Question 8

One component I developed was the map.js file. This file contains functions useful for mapping multiple addresses or routes onto a map. To adapt the code to a new project, I may need to change the names of the object properties. I could reuse that component in any project that requires the generation of maps.

### Question 9

Software projects run into many problems when they deploy. Many of these problems boil down to concurrency or scaling. When code actually deploys, many users will participate simultaneously. In our project, we never rigorously tested our platform with many concurrent users. If an admin deleted a user during an order, problems could occur. In terms of scaling, our program could have inefficiencies that do not cause problems until the database grows or many users strain the servers. 

### Question 10

.NET MVC implements a distributed system becuase code runs on different machines and interacts. For example, when a customer places an order, their machinee sends an HTTP POST to the Optimal Hacks server. The server processes the request to place the order onto the server. 

### Question 11

A Service Oriented Architecture encapsulates functionality and interacts with client processes through a well-defined protocall. In our project, a user needs to access the Optimal Hacks server through our website. If our project utilized a service oriented paradaigm, then any application could intereact with our servers. 

Service oriented architectures create self-contained functionality that can interact with a variety of other programs. Since the services focus on one area of functionality, they do not have as much bloat as a single program that tries to do everything. 

Further, since service oriented architectures generally create an API prior to development, multiple teams could develop multiple services which integrate nicely at the end of the project.

### Question 12

In our project, my group used git to separate each developer's work. Whenever a new feature needed development, the programmer created a branch to develop that feature. Towards the end of each sprint, every developer merged back into develop. When the sprint finished, the team ensured that develp worked properly. Finally, teh team merged develop into master.

### Question 13

An error occurs when the software outputs an incorrect result. For example, if an ATM outputs $10 instead of $20, an error occured. While the user still received some money, the user did not receive the correct amount of money. A failure occurs when the system cannot perform the desired functionality at all. So, if the ATM caught fire and output no money, and failure occured.

### Question 14

Problems
1. Unmotivated team members.
2. Failure to meet requirements in a timely manner.
3. Changing customer expectations.

Solutions
1. Figure out what motivates individual team members. Depending on what interests the programmer, consider providing that programmer with different work.
2. Remove unnecessary requirements and focus on the most important ones.
3. Depending on the terms of the contract, remind the customer what they paid your team to build. If they pay hourly and frequently change their minds, that costs them more than it hurts you.

### Question 15

The code review process helps ensure a quality codebase. When every line of code has multiple people looking at it, many flaws can get fixed. Static analysis tools are products that ensure quality code. When the program can review code for potential errors, code quality increases. 
