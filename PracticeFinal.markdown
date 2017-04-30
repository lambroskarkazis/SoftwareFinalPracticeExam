# RAIK 383H: Software Engineering Practice Final
#### Spring 2017
#### Professor Mihaela Bobaru
#### Author Lambros Karkazis

### Question 1
Describe steps which your group took to manage complexity during your project.

### Question 2
What types of software projects benefit from a plan-driven approach? Which projects benefit from an agile approach?

### Question 3
You work as a software engineer at Blackboard. You develop the backend of the learning management software. Your summer intern gives you the following code...

```C#
public class Student extends Person {
	private Enumerable<CourseResult> completedCourses { get; set; }
	private Enumerable<Course> currentCourses { get; set; }

	// Other student related code here...

	public void FinishSemester() {
		completedCourses.append(currentCourses.getResults());
	}
	
	public void AddCourse(Course newCourse) {
		currentCourses.append(course);
	}
}
```

How would you compose a component test to ensure that these functions work together? What potential problems could arise from this implementation? (Note: component-level testing checks the interaction between functions.)

### Question 4
Why do many software projects begin with data modeling?

### Question 5
Provide an example of both a functional and non-functional requirement to illustrate the difference between the two.

### Question 6
Explain the concepts of high cohesion and loose coupling. Describe why these concepts help software development.

### Question 7
What benefits did .NET MVC bring to your project? What drawbacks did .NET MVC bring to your project?

### Question 8
Describe one component of your final project that you could reuse in another system. How would you reuse this component? 

### Question 9
How might your project's software need to change if you actually deployed it? What software problems can production bring to light? 

### Question 10
How does .NET MVC implement a distributed system? (Hint: think about which code runs on which machine)

### Question 11
Define Service Oriented Architectures and describe their benefits.

### Question 12
How did you use git during your project? How did your group structure your branches?

### Question 13
What is the difference between an error and a failure in software dependability?

### Question 14
Name three problems faced by project managers and a solution to each.

### Question 15
Software teams generally try to ensure quality through process, product or some combination of both. Describe one process and one product that could ensure quality software. 
