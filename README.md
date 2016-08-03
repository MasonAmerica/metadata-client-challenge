# Metadata Client Programming Exercise

## Problem Statement
This exercise covers the creation of a simple command line (terminal) client that is responsible for performing the following operations:

1. Read a supplied Android APK file as input.
2. Inspect it to infer metadata about the APK, such as the package name, version name and version code.
3. Construct a document containing this information.
4. Save it out to a file as well as print it out to the console.

### Requirements
1. The constructed document must contain at least 5 unique pieces of useful information (your choice) about the APK, but _must_ include the **package name** and the **version code**.
2. The tool must be runnable from a command line in such a way that any dependencies needed are already present. If dependencies are required to be pre-installed, it is acceptable to supply a document named `README.dep` containing notes on how to accomplish this, or to print a message indicating what dependencies are needed and how they are to be installed.
3. The tool must be runnable from within a `bash` or `zsh` terminal.
4. You are allowed to include external libraries as part of this project as long as their source is also available and can be shared. If you do so, please include a `CREDITS` file containing links to the source and/or binary artifacts or project page.


___
Please do not hesitate to get in touch with your Mason engineer contact(s) if you have _any_ questions.
___


## Command Line Specification
The provided tool must support the following specification:

```
$ mdcli --help

Metadata Client version 1.0.

Usage:

mdcli --input <infilename> --package <package> [--output <outfilename>]

  --input <infilename>     Path to the APK file to be used as input
  --package <package>      Package name expected (validated against the input APK file)
  --output <outfilename>   Path to the output file created using metadata read from the APK

  [Additional options here if any]

```

## Notes

A Java project (using [Gradle](http://www.gradle.org)) is included as a starter. You are under no obligation to build a Java client; other languages are acceptable if you are able to find supporting libraries.

While designing your client, please consider that this client may potentially need to feed the inferred metadata to a backend server in a future release.


## Legal
Please note that any code, documentation and/or artifacts you submit as part of this exercise becomes the property of Mason America Inc. which reserves the right to use or modify this code as seen fit.
