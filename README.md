# Java-Resource

# Java Features (Java 8 → Java 24)

This document provides a structured overview of Java features from **Java 8** to **Java 24** in a table format.  
Each feature includes its **type** and **purpose/use case**.

---

## Java 8 Features

| Version | Feature Name                                   | Type                  | Purpose / Use Case                                           |
|---------|-----------------------------------------------|-----------------------|-------------------------------------------------------------|
| Java 8  | Lambda Expressions                             | Final                 | Functional-style programming; simplify anonymous classes     |
|         | Stream API                                     | Final                 | Process collections declaratively (map, filter, reduce)      |
|         | Default & Static Methods in Interfaces         | Final                 | Add new methods to interfaces without breaking existing code |
|         | Functional Interfaces + `@FunctionalInterface` | Final                 | Support lambdas with single abstract method interfaces       |
|         | Optional<T>                                    | Final                 | Avoid `null`; represent optional values clearly              |
|         | Date & Time API (`java.time`)                  | Final                 | Modern, immutable time/date handling                         |
|         | Nashorn JS Engine                              | Final (removed later) | Embed JS inside Java apps                                    |
|         | Repeating Annotations                          | Final                 | Apply same annotation multiple times                         |
|         | Method References                              | Final                 | Pass methods like lambdas: `ClassName::methodName`           |
|         | Collectors                                     | Final                 | Combine stream results — e.g., `Collectors.toList()`         |

---

## Java 9 Features

| Version | Feature Name                     | Type            | Purpose / Use Case                                           |
|---------|----------------------------------|-----------------|-------------------------------------------------------------|
| Java 9  | JShell (REPL)                    | Tool            | Interactive shell for experimenting with Java code           |
|         | Module System (Project Jigsaw)   | Language/Module | Modularize applications and JDK itself                       |
|         | Private Methods in Interfaces    | Language        | Allow code reusability within interfaces                     |
|         | Factory Methods for Collections  | API             | Easy immutable collections (`List.of()`, `Set.of()`)         |
|         | Process API Updates              | API             | Better control and management of OS processes                |
|         | Try-With-Resources Enhancement   | Language        | Simplified resource management                               |
|         | Compact Strings                  | JVM             | Reduce memory usage of String class                          |
|         | HTTP/2 Client (Incubator)        | API/Networking  | Support for HTTP/2 protocol                                  |
|         | Multi-Release JARs               | Packaging       | Create JARs targeting multiple Java versions                 |

---

## Java 10 Features

| Version | Feature Name              | Type       | Purpose / Use Case                                           |
|---------|---------------------------|------------|-------------------------------------------------------------|
| Java 10 | Local Variable `var`      | Language   | Simplify variable declarations with type inference           |
|         | Application Class-Data Sharing (AppCDS) | Performance | Improve startup performance by sharing class metadata across JVMs |
|         | Parallel Full GC for G1   | GC         | Improves performance of G1 garbage collector                 |
|         | Root Certificates         | Security   | Standard root certificates bundled with JDK                  |
|         | Thread-Local Handshakes   | JVM        | Stop individual threads without stopping all threads         |
|         | Time-Based Release Versioning | Release Model | New versioning scheme (feature releases every 6 months)  |

---

## Java 11 Features (LTS)

| Version | Feature Name                         | Type            | Purpose / Use Case                                           |
|---------|--------------------------------------|-----------------|-------------------------------------------------------------|
| Java 11 | `var` in Lambda Parameters           | Language        | Type inference in lambda expressions                         |
|         | HTTP Client (Standardized)           | API/Networking  | Standard HTTP/2 client                                       |
|         | `String` Methods (`isBlank`, `lines`, `strip`, `repeat`) | API | Convenience methods for common string operations |
|         | File Methods (`readString`, `writeString`) | API          | Easier file I/O                                              |
|         | Local-Variable Syntax for Lambda     | Language        | Simplified lambda expressions                                |
|         | Flight Recorder & Mission Control    | Tooling         | Low-overhead profiling and diagnostics                       |
|         | Epsilon GC (No-Op)                   | GC              | Useful for testing without GC overhead                       |
|         | Deprecate Nashorn JS Engine          | Deprecation     | Mark Nashorn for future removal                              |
|         | Deprecate Pack200 Tools              | Deprecation     | Mark Pack200 compression for removal                         |

---

## Java 12 Features

| Version | Feature Name                   | Type                  | Purpose / Use Case                                           |
|---------|--------------------------------|-----------------------|-------------------------------------------------------------|
| Java 12 | Switch Expressions (Preview)   | Language (Preview)    | Simplify `switch` with expressions                          |
|         | JVM Constants API              | JVM/API               | Access to constant pool in a structured way                 |
|         | Shenandoah GC (Experimental)   | GC                    | Low-pause-time garbage collector                            |
|         | Microbenchmark Suite           | Tooling               | Framework for writing JVM benchmarks                        |
|         | Abortable Mixed Collections in G1 | GC                  | Allow aborting garbage collection to improve latency        |
|         | Default CDS Archives           | Performance           | Improve startup with default shared class data              |

---

## Java 13 Features

| Version | Feature Name                   | Type                  | Purpose / Use Case                                           |
|---------|--------------------------------|-----------------------|-------------------------------------------------------------|
| Java 13 | Text Blocks (Preview)          | Language (Preview)    | Multi-line string literals with cleaner syntax               |
|         | Switch Expressions (2nd Preview) | Language (Preview)   | Refined preview of switch expressions                       |
|         | Dynamic CDS Archives           | Performance           | Improve startup with dynamically generated shared class data |
|         | Legacy Socket API Replacement  | API                   | Replace outdated socket implementation                      |

---

## Java 14 Features

| Version | Feature Name                                | Type                  | Purpose / Use Case                                                                 |
|---------|---------------------------------------------|-----------------------|-----------------------------------------------------------------------------------|
| Java 14 | Switch Expressions (Final)                  | Language (Final)      | Finalized switch expressions with concise syntax and `yield` keyword               |
|         | Records (Preview)                           | Language (Preview)    | Immutable data carrier classes with minimal boilerplate                            |
|         | Pattern Matching for `instanceof` (Preview) | Language (Preview)    | Simplify `instanceof` checks by eliminating explicit casting                       |
|         | Helpful NullPointerExceptions               | JVM Improvement       | More detailed error messages with variable/field name causing NPE                  |
|         | JFR Event Streaming                         | Tooling/API           | Continuous data streaming from Java Flight Recorder                               |
|         | Packaging Tool (Incubator)                  | Tooling (Incubator)   | Package self-contained Java applications for OS platforms                          |
|         | NUMA-Aware Memory Allocation (G1 GC)        | JVM/GC Improvement    | Optimize memory allocation on NUMA-based systems                                   |
|         | Foreign-Memory Access API (Incubator)       | API (Incubator)       | Safe, efficient access to native memory outside Java heap                          |

---

## Java 15 Features

| Version | Feature Name                   | Type                  | Purpose / Use Case                                           |
|---------|--------------------------------|-----------------------|-------------------------------------------------------------|
| Java 15 | Text Blocks (Final)            | Language              | Finalized multi-line string literals                        |
|         | Sealed Classes (Preview)       | Language (Preview)    | Restrict inheritance to defined subclasses                  |
|         | Records (Second Preview)       | Language (Preview)    | Data carrier classes with minimal boilerplate (refined)      |
|         | Hidden Classes                 | JVM/Runtime           | For frameworks to generate classes dynamically              |
|         | Pattern Matching for `instanceof` (Second Preview) | Language (Preview) | Refined pattern matching for instanceof                     |
|         | ZGC: Production Ready          | Garbage Collector     | Z Garbage Collector moves to production status              |
|         | Shenandoah: Production Ready   | Garbage Collector     | Low-pause-time GC ready for production                      |
|         | Nashorn JS Engine Removal      | Removal               | Remove Nashorn (deprecated earlier)                         |
|         | RMI Activation Removal         | Removal               | Remove outdated RMI Activation system                       |

---

## Java 16 Features

| Version | Feature Name                         | Type                  | Purpose / Use Case                                           |
|---------|--------------------------------------|-----------------------|-------------------------------------------------------------|
| Java 16 | Records (Final)                      | Language              | Immutable data classes with minimal code                     |
|         | Pattern Matching for `instanceof` (Final) | Language           | Finalized simplification for instanceof + casting           |
|         | Sealed Classes (Second Preview)      | Language (Preview)    | Refined sealed classes                                       |
|         | JEP 338: Vector API (Incubator)      | API/Performance       | SIMD computations for better math performance               |
|         | Strong Encapsulation of JDK Internals| JVM/Modules           | Restrict illegal reflective access                          |
|         | Packaging Tool (Incubator → Final)   | Tooling               | Create native app installers                                |
|         | Unix-Domain Socket Channels          | API/Networking        | Faster inter-process communication                          |

---

## Java 17 Features (LTS)

| Version | Feature Name                   | Type                  | Purpose / Use Case                                           |
|---------|--------------------------------|-----------------------|-------------------------------------------------------------|
| Java 17 | Sealed Classes (Final)         | Language              | Finalized inheritance control                               |
|         | Pattern Matching for `switch` (Preview) | Language (Preview) | Extended pattern matching to switch statements              |
|         | Strongly Encapsulate JDK Internals | JVM                  | Fully prevent reflective access                             |
|         | Restore Always-Strict Floating Point | Language            | Consistent floating-point operations                       |
|         | Deprecate Security Manager      | Deprecation           | Begin removal of legacy security manager                    |
|         | New macOS Rendering Pipeline    | Performance           | Use Metal API instead of old pipeline                       |
|         | Enhanced Pseudo-Random Number Generators | API              | More flexible random number APIs                           |
|         | Context-Specific Deserialization Filters | Security API      | Prevent unsafe deserialization                             |

---

## Java 18 Features

| Version | Feature Name                   | Type                  | Purpose / Use Case                                           |
|---------|--------------------------------|-----------------------|-------------------------------------------------------------|
| Java 18 | Simple Web Server              | Tooling               | Lightweight HTTP server for prototyping and testing          |
|         | UTF-8 by Default               | Language              | Default character set changed to UTF-8                       |
|         | Vector API (Second Incubator)  | API/Performance       | Improved vectorized computation                              |
|         | Internet-Address Resolution SPI| Networking API        | Custom resolvers for hostnames                              |
|         | Code Snippets in Javadoc       | Tooling               | Better documentation with executable examples               |

---

## Java 19 Features

| Version | Feature Name                                | Type                  | Purpose / Use Case                                           |
|---------|---------------------------------------------|-----------------------|-------------------------------------------------------------|
| Java 19 | Virtual Threads (Preview)                   | Concurrency/Project Loom | Lightweight threads for high scalability                  |
|         | Structured Concurrency (Incubator)          | Concurrency           | Simplified task grouping for multithreading                 |
|         | Record Patterns (Preview)                   | Language (Preview)    | Deconstruct record objects easily                           |
|         | Pattern Matching for `switch` (Third Preview)| Language (Preview)   | Refined switch pattern matching                             |
|         | Foreign Function & Memory API (Preview)     | API/Interop           | Safer native memory and function interop (Project Panama)   |
|         | Vector API (Third Incubator)                | API/Performance       | Further vector API improvements                             |

---

## Java 20 Features

| Version | Feature Name                                | Type                  | Purpose / Use Case                                           |
|---------|---------------------------------------------|-----------------------|-------------------------------------------------------------|
| Java 20 | Scoped Values (Incubator)                   | Concurrency/Memory    | Immutable, safer alternative to ThreadLocal                  |
|         | Record Patterns (Second Preview)            | Language (Preview)    | Refined record pattern matching                             |
|         | Pattern Matching for `switch` (Fourth Preview)| Language (Preview)   | Enhancements to switch pattern matching                     |
|         | Foreign Function & Memory API (Second Preview)| API/Interop          | Updated API for native interop                              |
|         | Virtual Threads (Second Preview)            | Concurrency           | More refinements to lightweight threads                     |
|         | Structured Concurrency (Second Incubator)   | Concurrency           | Refinements for structured concurrency                      |

---

## Java 21 Features (LTS)

| Version | Feature Name                                | Type                  | Purpose / Use Case                                           |
|---------|---------------------------------------------|-----------------------|-------------------------------------------------------------|
| Java 21 | String Templates (Preview)                  | Language (Preview)    | Embed expressions in strings safely                         |
|         | Sequenced Collections                       | Collections API       | Provide consistent iteration order                          |
|         | Generational ZGC                            | GC                    | Adds generational model to ZGC                              |
|         | Record Patterns (Final)                     | Language              | Deconstruction of record values                             |
|         | Pattern Matching for `switch` (Final)       | Language              | Finalized pattern-based branching                           |
|         | Foreign Function & Memory API (Final)       | API/Interop           | Finalized native interop API                                |
|         | Unnamed Patterns and Variables (Preview)    | Language (Preview)    | Ignore variables with `_`                                   |
|         | Virtual Threads (Final)                     | Concurrency           | Finalized lightweight threads                               |
|         | Unnamed Classes & Instance Main (Preview)   | Language (Preview)    | Simplify entry-point coding                                 |
|         | Scoped Values (Preview)                     | Concurrency/Memory    | Refined thread-shared immutable values                      |
|         | Vector API (Sixth Incubator)                | API/Performance       | SIMD operations improvement                                 |
|         | Deprecate Windows 32-bit x86 Port           | Deprecation           | Drop legacy platform support                                |

---

## Java 22 Features

| Version | Feature Name                                | Type                  | Purpose / Use Case                                           |
|---------|---------------------------------------------|-----------------------|-------------------------------------------------------------|
| Java 22 | Region Pinning for G1                       | GC                    | Improve G1 GC latency                                       |
|         | Statements before `super(...)` (Preview)    | Language (Preview)    | More flexible constructor initialization                    |
|         | Foreign Function & Memory API (Final)       | API/Interop           | Finalized native interop API                                |
|         | Unnamed Variables (Final)                   | Language              | Finalized `_` variables                                     |
|         | Class-File API (Preview)                    | API (Preview)         | Parse/transform `.class` files                             |
|         | Multi-File Source Program Launch (Preview)  | Tooling (Preview)     | Run multi-file source directly                              |
|         | String Templates (Second Preview)           | Language (Preview)    | Refined string templates                                    |
|         | Vector API (Seventh Incubator)              | API/Performance       | SIMD improvements                                           |
|         | Stream Gatherers (Preview)                  | Streams API (Preview) | More flexible stream transformations                        |
|         | Structured Concurrency (Second Preview)     | Concurrency           | Refinement for structured concurrency                       |
|         | Implicitly Declared Classes (Second Preview)| Language (Preview)    | Continued simplification for entry programs                 |
|         | Scoped Values (Second Preview)              | Concurrency           | Further refinements                                         |
|         | Class-File API (Second Preview)             | API (Preview)         | More refinements                                            |
|         | Markdown Javadoc (Preview)                  | Documentation         | Support for Markdown in Javadoc                             |

---

## Java 23 Features

| Version | Feature Name                                | Type                  | Purpose / Use Case                                           |
|---------|---------------------------------------------|-----------------------|-------------------------------------------------------------|
| Java 23 | Stream Gatherers (Preview)                  | Streams API (Preview) | Custom stream aggregations                                  |
|         | Scoped Values (Second Preview)              | Concurrency           | Safer alternative to ThreadLocal                            |
|         | Class-File API (Preview)                    | API (Preview)         | Parse/transform `.class` files                             |
|         | String Templates (Third Preview)            | Language (Preview)    | More refinements                                            |
|         | Structured Concurrency (Fourth Incubator)   | Concurrency           | Better concurrent task handling                            |
|         | Foreign Function & Memory API (Seventh Incubator)| API/Interop        | Refined FFM API                                             |

---

## Java 24 Features

| Version | Feature Name                                | Type                  | Purpose / Use Case                                           |
|---------|---------------------------------------------|-----------------------|-------------------------------------------------------------|
| Java 24 | Generational Shenandoah (JEP 404)           | GC (Experimental)     | Generational mode for Shenandoah GC                         |
|         | Compact Object Headers (JEP 450)            | JVM (Experimental)    | Reduce object header size                                   |
|         | Restrict JNI Usage (JEP 472)                | Deprecation           | Prepare to limit unsafe JNI usage                           |
|         | Late Barrier Expansion for G1 (JEP 475)     | GC Performance        | Optimize G1 GC barrier expansion                            |
|         | Key Derivation API (JEP 478)                | Security API (Preview)| Add secure key derivation mechanism                        |
|         | Remove Windows 32-bit x86 Port (JEP 479)    | Removal               | Remove legacy 32-bit x86 port                               |
|         | AOT Class Loading & Linking (JEP 483)       | Performance           | Improve startup with pre-linked classes                     |
|         | Class-File API (JEP 484)                    | API (Final)           | Official `.class` file API                                  |
|         | Stream Gatherers (JEP 485)                  | Streams API (Final)   | Stateful stream operations                                  |
|         | Remove Security Manager (JEP 486)           | Removal               | Remove legacy security model                                |
|         | Scoped Values (JEP 487)                     | Concurrency (Preview) | Immutable thread-shared values                              |
|         | Primitive Patterns (JEP 488)                | Language (Preview)    | Support for primitives in pattern matching                  |
|         | Vector API (JEP 489)                        | API/Performance       | SIMD vector improvements                                    |
|         | Remove Non-Generational ZGC (JEP 490)       | GC Removal            | Keep only generational ZGC                                  |
|         | Virtual Thread Synchronization (JEP 491)    | Concurrency Fix       | Avoid pinning in synchronized blocks
