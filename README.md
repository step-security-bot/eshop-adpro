Nama: Carleano Ravelza Wongso

NPM: 2306213022

Kelas: Adpro-B

# Reflection 1: Coding Standard and Secure Coding
> You already implemented two new features using Spring Boot. Check again your source code and evaluate the coding standards that you have learned in this module. Write clean code principles and secure coding practices that have been applied to your code. If you find any mistake in your source code, please explain how to improve your code

##  Coding Standard

### Separation of Concerns

I have structured the application following the layered architecture, ensuring that responsibilities are well-separated across different components:

- Controller Layer: Handles HTTP requests and responses. 
- Service Layer: Contains business logic and interacts with the repository.
- Repository Layer: Manages entities

### Meaningful Naming

I use descriptive and intuitive names for variables, methods, classes, and packages to improve readability.

### Consistent Formatting and Indentation

I maintain a uniform coding style by:
- Using proper indentation, spacing, and line breaks.
- Following Java conventions (e.g., class names in PascalCase, variables in camelCase).
- Keeping method length manageable and avoiding long parameter lists.

## Secure Coding Practices

### Input Validation

I ensure that user input is validated to prevent security vulnerabilities.

### Error Handling

I implement structured exception handling to prevent system crashes and information leakage.

# Reflection 2: Testing

## Unit Testing

> After writing the unit test, how do you feel? How many unit tests should be made in a class? How to make sure that our unit tests are enough to verify our program? It would be good if you learned about code coverage. Code coverage is a metric that can help you understand how much of your source is tested. If you have 100% code coverage, does that mean your code has no bugs or errors? 

After writing unit tests, I feel more confident about my code's reliability. Unit tests help ensure that individual components of the program function as expected and make debugging easier by pinpointing failures early. They also provide a safety net when making changes, reducing the risk of unintended side effects.

### Number of Unit Tests

The number of unit tests in a class depends on the complexity of the class and its methods. Generally, each method should have at least one test case, but multiple tests should be written to cover different input scenarios, edge cases, and error handling. 

### Ensuring Unit Tests Are Sufficient

To ensure that unit tests adequately verify the program, I considered the following:
- Code Coverage
- Edge Cases
- Mutation Testing

### Does 100% Code Coverage Mean No Bugs?

No, 100% code coverage does not guarantee that the code is free of bugs or errors. Code coverage only indicates which lines of code were executed during testing but does not ensure logical correctness. Therefore, while high code coverage is beneficial, it should be complemented with integration testing, end-to-end testing, and real-world testing to ensure software reliability.

## Functional Testing

> Suppose that after writing the CreateProductFunctionalTest.java along with the corresponding test case, you were asked to create another functional test suite that verifies the number of items in the product list. You decided to create a new Java class similar to the prior functional test suites with the same setup procedures and instance variables. <br><br> What do you think about the cleanliness of the code of the new functional test suite? Will the new code reduce the code quality? Identify the potential clean code issues, explain the reasons, and suggest possible improvements to make the code cleaner!

The new functional test suite for verifying product list items raises several clean code concerns:

- Code Duplication
- Hard Coded Values

To improve the functional test, we can do the following:
- Create a base class for the tests
- Making sure we get our constants values (e.g. Base URL, product ID, product name) come from one source (e.g. env file).