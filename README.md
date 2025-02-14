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
