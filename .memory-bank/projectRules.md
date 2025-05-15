# projectRules.md: <Replace with a current Project Name>

## 0. Project-Specific Intelligence
*   <here we will add project-specific intelligence>

## 1. Fundamental Practices

*   Write clean, simple, and readable code.
*   Implement features in the simplest way that fulfills the requirements.
*   Keep files small and focused (e.g., <300 lines); if a file grows too large, consider refactoring.
*   Test after every meaningful change.
*   Focus on core functionality before optimizing.
*   Use clear and consistent naming conventions (e.g., `_callback` suffix for callback methods, or other project-agreed conventions).
*   Strive for a modular architecture with single-responsibility components.

## 2. Error Fixing & Prevention

*   Explain problems in plain English before attempting fixes.
*   Consider multiple potential causes before fixing; avoid jumping to conclusions.
*   Make only the minimal necessary changes to address an issue.
*   Add error prevention patterns after resolution where appropriate.
*   When fixing an issue, error, or bug, proactively consider where similar issues might exist elsewhere in the codebase and address them comprehensively if feasible.
*   Implement robust error handling using `try-except` blocks or equivalent language constructs, and log errors effectively.

## 3. Building Process & Refactoring

*   Provide clear testing instructions or automated tests to verify new features.
*   Prefer simple solutions and established patterns over overly complex frameworks or premature optimization.
*   Refactor mercilessly while maintaining functionality to improve code quality and maintainability.

## 4. Comments & Documentation

*   Include a header comment in every file with its relative path from project root and a summary of its purpose.
*   Document complex logic, inter-module interactions (e.g., callbacks, API contracts), and asynchronous operations clearly.
*   Preserve existing comments unless they are obsolete or incorrect.
*   Maintain change rationales in comments or commit messages.
*   Use simple language and short sentences in comments.

## 5. Cross-Cutting Concerns

*   Prioritize readability and maintainability, especially in modular systems.
*   Maintain consistency across the codebase (e.g., how settings are accessed, how logging is performed, coding style).
*   Clearly explain the logic in plain language where necessary.

## 6. Technology-Specific Considerations (General Examples)

*   **Asynchronous Operations:** When using asynchronous programming (e.g., `asyncio`, Promises, Threads), ensure proper management of event loops, tasks, and concurrency controls (e.g., Semaphores, Mutexes).
*   **Modular Communication:** Define clear interfaces and communication patterns between modules (e.g., callbacks, events, message queues, API calls).
*   **Configuration Management:** Implement a system for managing application settings (e.g., using configuration files, environment variables) with clear access patterns.
*   **Logging:** Establish a centralized logging mechanism with appropriate log levels and handlers for different outputs (e.g., console, file, UI).
*   **State Management:** Clearly define how application state is managed, especially in UI applications or distributed systems.

## 7. Agent Interaction

*   When updating a "Memory Bank" or similar project knowledge base, ensure all relevant core files are reviewed and updated to reflect the current project state, especially after major changes or refactoring.
*   Every answer should start with a line "Okey-dokey! 😉" followed by a blank line before any further text.
