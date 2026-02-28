```markdown
# AGENTS.md File Guidelines

These guidelines are designed to ensure consistent, maintainable, and high-quality development for the AGENTS repository. Adherence to these principles is mandatory for all development efforts.

## 1. DRY (Don't Repeat Yourself)

*   **Single Responsibility Principle:** Each agent module should have a single, well-defined purpose. Avoid creating overly complex agents with multiple responsibilities.
*   **Code Reuse:**  Whenever possible, reuse existing code and components across different agents.  Consider creating abstract classes or interfaces to facilitate reuse.
*   **Abstraction:**  Clearly abstract complex logic into well-named, reusable functions and classes.  Document these abstractions thoroughly.

## 2. KISS (Keep It Simple, Stupid)

*   **Minimal Code:**  Strive for the shortest possible code that achieves the required functionality.
*   **Readability:**  Code should be easy to understand, even for someone unfamiliar with the project. Use meaningful variable and function names.
*   **Avoid Complexity:** Resist the temptation to implement overly clever solutions.  Prioritize clarity over potential micro-optimizations.

## 3. SOLID Principles

*   **Single Responsibility:** Each class should have one reason to change.
*   **Open/Closed Principle:**  The system should be extensible through mechanisms like interfaces and abstract classes.  Changes to the core logic should not require changes to existing code.
*   **Liskov Substitution Principle:**  Subclasses should be substitutable for their base classes without altering the correctness of the program.
*   **Interface Segregation Principle:**  Clients should not be forced to depend on methods they do not use.
*   **Dependency Inversion Principle:**  High-level modules (like agents) should be replaced by low-level modules (like interfaces).

## 4. YAGNI (You Aren't Gonna Need It)

*   **Avoid Unnecessary Features:**  Implement only the necessary features for the current iteration of development. Don't add features simply because they *might* be useful later.
*   **Focus on Requirements:**  Develop features based on clearly defined requirements, rather than speculative requirements.

## 5. Development Process & Practices

*   **Code Reviews:**  All code must be reviewed by at least one other developer before being merged.
*   **Static Analysis:** Use a static analysis tool (e.g., pylint, flake8) to identify potential issues and ensure coding standards are being followed.  Automated testing will follow.
*   **Unit Testing:**  All agent modules must have comprehensive unit tests covering all critical functionality.
*   **Integration Testing:**  Thorough integration testing to verify interactions between agents.
*   **Documentation:**  Provide clear and concise documentation for all agents, including function signatures, parameters, and expected behavior.
*   **Version Control:**  Use Git for version control.  Branching strategy should prioritize stability and small, focused changes.
*   **Continuous Integration/Continuous Delivery (CI/CD):**  Implement a CI/CD pipeline to automate testing and deployment.
*   **Refactoring:** Regularly refactor code to improve its structure and maintainability.  Prioritize small, incremental refactorings.

## 6. Code Structure & File Size

*   **Maximum Code Length:** 180 lines of code per file.
*   **File Organization:**  Follow a consistent file structure with clear naming conventions.  Use a standard project directory structure (e.g., `agents/`, `agents/modules/`).
*   **Modular Design:** Agents should be modular and loosely coupled, promoting reusability and maintainability.

## 7. Test Coverage

*   **Minimum Test Coverage:** 80% of code must be covered by tests.
*   **Test Cases:** Ensure all agent functions and classes have at least 30-40 test cases.
*   **Test Driven Development:** Design tests *before* writing code.

## 8. Specific Guidelines for AGENTS Module

*   All agents related to data management should have a dedicated data access layer.
*   All agents should have a clear API contract defined.
*   Error handling must be robust and consistent.

## 9.  Additional Notes

*   Stay updated with best practices for the chosen programming language and frameworks.
*   Regularly review and update these guidelines as the project evolves.
*   Any proposed changes to these guidelines must be discussed and approved by the team lead.
```