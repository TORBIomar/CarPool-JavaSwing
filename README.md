# Carpool-Swing

Desktop carpool management application built with Java Swing.

## Features

- Swing-based desktop UI for admins, drivers, and passengers
- User registration/login and role-based dashboards
- Trip management, reservations, and reviews
- JDBC-based persistence with MySQL

## Project Structure

- `src/` - Java source code
- `lib/` - external JAR dependencies
- `NetBeansProject/` - NetBeans project metadata
- `build.xml` - Apache Ant build script
- `manifest.mf` - JAR manifest metadata

## Requirements

- Java JDK 8 or higher
- MySQL database configured for the app
- IntelliJ IDEA or any Java IDE (optional)

## Run in an IDE

1. Open the project in your Java IDE.
2. Add both JARs from `lib/` to the project classpath.
3. Set `app.Main` as the entry point.
4. Run the application.

## Build with Ant (NetBeans-compatible)

From the repository root:

```bash
ant clean
ant compile
ant run
```

## Run from Terminal

From the repository root:

```bash
javac -cp "lib/*" -d out src/app/Main.java src/ui/*.java src/utils/*.java
java -cp "out;lib/*" app.Main
```

Note for Unix/macOS users: replace `;` with `:` in the `java -cp` command.

## Repository Hygiene

- Generated files are intentionally ignored (`build/`, `out/`, `.class`, IDE private metadata).
- Do not commit IDE-local settings or compiled artifacts.
