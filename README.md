# Work-in-progress

**TODOS**

* Build shared code JAR
* Build JRE lib
* Build Android lib
* Build sample app
* Use gradle for the JRE code too (instead of ant)?
* All the TBDs below...
* Get the Android lib out of the sample app?



## Getting started

### Using the Android library

**TBD**

### Using the JRE library

**TBD**

## Development info

### Building the libraries

```bash
make build   # builds Android and JRE versions
```

### Publishing the libraries

**TBD**

###  Directory structure

*Note: the below is a target...the code's not there yet...*

```
Makefile                   <- Top-level Makefile to encapsulate tools specifics
settings.gradle            <- definition of sub-projects

build.gradle               <- main Gradle build file, dependencies & plugins
gradlew                    <- script that will run Gradle on Unix systems
gradlew.bat                <- script that will run Gradle on Windows
gradle                     <- local gradle wrapper

common/
    build.gradle           <- Gradle build file for common project
    src/                   <- Source for shared code
android/
    build.gradle           <- Gradle build file for Android lib
    AndroidManifest.xml    <- Android specific config
    src/                   <- Source for Android lib
    sample/                <- sample app
jre/
    build.gradle           <- Gradle build file for the html project*
    src/                   <- Source for JRE Java library
    sample/                <- sample app
```
