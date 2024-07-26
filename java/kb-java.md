# Code Style
Objective: Ensure consistent code style for readability and maintainability.

## Code Formatting
Resource: [Google Java Style Guide](https://google.github.io/styleguide/javaguide.html)
- Follow the Google Java Style Guide for consistent formatting.
- Use consistent indentation (4 spaces).
- Keep line length to a maximum of 100 characters.

## Naming Conventions
Resource: [Java Code Conventions](https://www.oracle.com/java/technologies/javase/codeconventions-namingconventions.html)
- Class names should be nouns in UpperCamelCase.
- Method names should be verbs in lowerCamelCase.
- Constants should be in UPPER_SNAKE_CASE.

## Comments and Documentation
Resource: [Effective Java by Joshua Bloch](https://kea.nu/files/textbooks/new/Effective%20Java%20%282017%2C%20Addison-Wesley%29.pdf)
- Use [Javadoc](https://en.wikipedia.org/wiki/Javadoc#Structure_of_a_Javadoc_comment) for public methods and classes.
- Write meaningful comments explaining the purpose of complex code blocks.

## Best Practices
Resource: [Effective Java by Joshua Bloch](https://kea.nu/files/textbooks/new/Effective%20Java%20%282017%2C%20Addison-Wesley%29.pdf)
- Avoid magic numbers; use constants.
- Favour immutability; use final where applicable.
- Use Optional to handle null values gracefully.
  
# Project Structure
Objective: Organise the project for scalability and maintainability using hexagonal architecture.

## Hexagonal Architecture Overview
Resource: [Hexagonal Architecture by Alistair Cockburn](https://alistair.cockburn.us/hexagonal-architecture/)
- Also known as ports and adapters architecture, it promotes separation of concerns and increases testability.

## Standard Directory Layout
Resource: [Hexagonal Architecture in Spring](https://alistair.cockburn.us/hexagonal-architecture/)
- Follow a structure that separates the core business logic from external dependencies

## Layered Structure

Resource: https://github.com/bukuwarung/edc-adapterConnect your Github account

### Domain Layer
Contains core business logic and domain models.

### Application Layer
Manages application-specific logic, DTOs, and services.

### Common Layer
Encapsulates utilities, constants & exceptions

### Adapters
Handles interactions with external systems, controllers, repositories, and configurations.

## Configuration Management
Resource: [Spring Boot Configuration](Spring Boot Configuration)
- Externalise configurations using application.properties or application.yml.
- Use profiles for different environments (dev, test, prod).