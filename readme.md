# Java CLI with Picocli

This project is a simple Command Line Interface (CLI) application built using Java and the Picocli framework. The application demonstrates the use of subcommands to print greeting and farewell messages.

## Project Structure

- `src/main/java/ch/heigvd/dai/Main.java`: The main entry point of the application.
- `src/main/java/ch/heigvd/dai/commands/Hello.java`: Subcommand to print a greeting message.
- `src/main/java/ch/heigvd/dai/commands/Goodbye.java`: Subcommand to print a farewell message.
- `pom.xml`: Maven configuration file.

## Prerequisites

- Java 21 or higher
- Maven 3.6.0 or higher

## Building the Project

To build the project, run the following command in the project root directory:

```sh
mvn clean package
```

This will compile the project and create a shaded JAR file in the `target` directory.

## Running the Application

To run the application, use the following command:

```sh
java -jar target/java-intellij-idea-and-maven-1.0-SNAPSHOT.jar <command> [options]
```

### Available Commands

- `hello`: Prints a greeting message.
- `goodbye`: Prints a farewell message.

### Command Options

#### `hello` Command

```sh
java -jar target/java-intellij-idea-and-maven-1.0-SNAPSHOT.jar hello [options]
```

Options:
- `-g`, `--greetings`: The greetings to address the user (default: Hello).

#### `goodbye` Command

```sh
java -jar target/java-intellij-idea-and-maven-1.0-SNAPSHOT.jar goodbye [options]
```

Options:
- `-f`, `--farewells`: The farewells to address the user (default: Goodbye).

## Examples

Print a greeting message:

```sh
java -jar target/java-intellij-idea-and-maven-1.0-SNAPSHOT.jar hello -g "Hi"
```

Print a farewell message:

```sh
java -jar target/java-intellij-idea-and-maven-1.0-SNAPSHOT.jar goodbye -f "See you"
```

## About this readme
This readme was partially generated using AI.
```

