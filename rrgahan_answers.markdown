## Q1 - Managing Complexity
One thing our group did to manage complexity was refactor our code throughout the project. We attempted to keep methods small and well documented, which made the code easier to understand. If a method grew to big, we would refactor by separating it into multiple smaller methods.
We also utilized git to manage complexity, specifically the Review function in Github. By requiring an `approval` review by a teammate, code was proof-read by at least one other set of eyes, which reduced on any unnecessary code being used.


## Q2 - Plan-Driven vs Agile
Plan-driven is best used for big projects. If there are a lot of requirements or moving pieces that rely on each other, having a well-written plan is helpful for scheduling. Plan-driven is also very helpful on teams where members are not centrally located.

Agile is great when the development must be rapid, incremental delivery is okay or expected, and the client is willing to be heavily involved throughout the process. Because it is a `quicker` process, changes can be implemented more quickly and with less cost than plan-driven.


## Q3 - Blackboard Code
**Testing**
You could start with a new student. Begin adding courses to their schedule using the `addCourse` method, then end the semester using the `finishSemester` method. If the whole test finishes with a satisfactory result, both methods work.

**Problems**
In my opinion, `completedCourses` should be an `Enumerable` of type `Course`. Different methods related to retrieving information/properties of the courses can be written as needed. When a semester if finished, `currentCourse` needs to be emptied. Depending on the rules of the school, enrolling in a class shouldn't necessarily mean the class is a current course.


## Q4 - Data Modeling
By beginning with data modeling, the dev team is able to see what types of interactions will be required between the different components. The models can be better created, as any repeating data can be consolidated into an inheritance class-type situation, or into it's own model that is a foreign key to other models. Another benefit is they know exactly how the classes will interact with each other, so adding methods becomes much easier. A final benefit is that by creating data models first, fewer migrations need to be made, which significantly cuts back on the physical pain conflicting migrations cause.


## Q5 - Functional/Non-Functional Requirements 
**Using adding a class as an example...**

*Functional:* Students should be able to enroll in a class for their next-semester schedule.

*Non-Functional:* Enrollment site should have 99% uptime during priority registration and 90% uptime during the rest of semester.

## Q6 - High Cohesion/Loose Coupling
*High Cohesion:* Methods in a class relate directly to the class itself. __within__
*Loose Coupling:* Class does not need much from another class. __amount__

## Q7 - .NET MVC
MVC provided a lot of structure for the project. Because it is a very well defined and well documented pattern, everyone on the team was on the same page with regards to where code should go (managers vs stores vs controllers). The testing framework that .NET uses also provided a lot of benefit because writing unit tests was very useful in ensuring the code we wrote was workable.

For this specific project, MVC had some drawbacks. Because the product was relatively simple and short term, all the structure provided by MVC wasn't necessary. It also made it overly complicated to implement small methods.

## Q8 - Reuse of Project
Within our project, route creation is probably the most useful part of code. It involves dividing unassigned orders into geographic clusters then finding the optimal route for driving. This is useful for any software that delivers using pickup and drop off locations. To prepare this code for reuse, we would bundle it up as a `NuGet` package. We could then reuse the package whenever needed by installing it then calling the respective methods. One thing that could be done to make it easier for reuse is create an `Index` method that takes in all the required parameters for any methods and then calls all the methods in order. By doing so, the user needs less knowledge of the package.

## Q9 - Going Live
One of the biggest issues with going live would be speed. Because there was not the non-functional requirement of timeliness, the product was not designed to be fast. This could be fixed for production by doing smarter database queries. We would also have to focus more on UI/UX to make the product more user friendly. Going live typically shifts the focus from functional to non-functional requirements. For example, scalability isn't a problem when running a local setup, but is a major focus when in production.

## Q10 - MVC Distributed?
idk

## Q11 - SOA
boy do I need to study

## Q12 - git
In theory, a new branch was created from `develop` for each feature. All the relevant work on the feature was done on that branch. When the dev was finished with it, he pushed it up and created a pull request. The PR was assigned to another dev who pulled the branch down and ran it locally on his machine. In practice, small features or fixes were implemented directly on the develop branch. Pull Requests were not always ran locally, which created issues when merged code didn't build properly. 

## Q13 - Error vs Failure
An error is something that goes wrong, but the system is able to continue functioning. Example: user inputs a date in the past, the form validation catches this __error__ and reloads the form with the error explained. A failure is something that breaks the system. For example, a failure could result from a 400 error when reaching out to an API.

## Q14 - PM
- Unmotivated developer: The project manager should set up a 1 on 1 with the dev to try to figure out why they are unmotivated. If the issue is solvable, the PM should fix it. An example of this would be if the dev is writing SQL queries but they prefer to do web design. If it is not solvable, such as the dev doesn't like the project but they are an integral part of the team, the PM needs to be sensitive to the dev. If possible, the PM should continue to meet with the dev to see if any small changes can be made to make the project more exciting, or else throughout the project explain to the dev how they are being benefited by being on the team.

- Talented developer on maternity/paternity leave: If possible, structure the project schedule so the developer's work is complete before they leave. Otherwise, the PM will need to look for a temporary replacement that will match both the culture and the skill of the dev.

- Dev team doesn't have consistent view of solution: This problem can be solved by having a full team meeting explaining the broad or most important requirements. Then have the team pitch their own ideas about the actual implementation so they are actually involved in the decision making process. By doing so, the team feels ownership over the product, which will generally lead to higher quality commitment *and* code. Another benefit of doing an all-hands meeting is each individual member has the opportunity to learn about the entire project which will give them insight on exactly how their section fits into the whole.

## Q15 - Process/Product
*Process:* Peer-reviewed code will really help with software quality. By requiring each pull request to be reviewed by another member of the dev team, simple mistakes can be caught before merging.

*Product:* Continuous Integration (CI) can be used to ensure the constant quality of the code. Depending on the type of CI, you can make sure the product builds successfully and/or all the tests pass. This catches any changes that affected unknown parts of the code.
