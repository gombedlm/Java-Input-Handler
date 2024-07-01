# Java SafeInput Handler

## Overview
Java SafeInput Handler is a robust utility designed to streamline and secure user input handling in Java applications. It offers a suite of tools to validate, sanitize, and process user input efficiently, reducing the risk of errors and vulnerabilities in your applications.

## Features
- **Input Validation**: Ensures user input meets specified criteria.
- **Input Sanitization**: Cleans user input to prevent injection attacks.
- **Error Handling**: Provides detailed error messages and logging.
- **Extensibility**: Easily extendable to add custom validation rules.


## Getting Started

### Prerequisites
- Java Development Kit (JDK) 8 or higher
- Maven or Gradle for dependency management (optional)

### Installation
1. Clone the repository:
    ```sh
    git clone https://github.com/gombedlm/Java-SafeInput-Handler.git
    ```
2. Navigate to the project directory:
    ```sh
    cd Java-SafeInput-Handler
    ```
3. Build the project in the directory you've been guided to using your preferred build tool (e.g., Maven, Gradle).

### Usage
Here's a simple example demonstrating how to use the SafeInput Handler in a Java application with many of its functions in use:

```java
import java.util.Scanner;
import com.safeinput.SafeInput;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        // Example usage of SafeInput methods
        String nonEmptyString = SafeInput.getNonZeroLenString(scanner, "Enter a non-empty string");
        int integer = SafeInput.getInt(scanner, "Enter an integer");
        double floatingPoint = SafeInput.getDouble(scanner, "Enter a decimal number");

        System.out.println("Entered String: " + nonEmptyString);
        System.out.println("Entered Integer: " + integer);
        System.out.println("Entered Double: " + floatingPoint);

        scanner.close();
    }
}
```

## Other Versions
### Python 
A Future Python Version will be implemented and linked here


