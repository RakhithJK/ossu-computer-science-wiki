# Core Programming

## Prerequisites
- Intro CS

## Resources

### Functional Computation
This section introduces you to a simple, foundational model of computation close to high school math.
If you've taken programming classes before, this programming model may surprise or confuse you.
We urge you to persevere as what you learn here will build a sound foundation for the rest of your studies.

Choose between the book or the two courses, which are based on the book.
The book is free, but the courses offer graded assessments if you're willing to pay.

| Format   | Resource                                                                                     | Use cases | Length    |
|----------|----------------------------------------------------------------------------------------------|-----------|-----------|
| `book`   | *[How to Design Programs](https://htdp.org/)* (Felleisen, Findler, Flatt, Krishnamurthi)     | `learn`   | 792 pages |
| `course` | [UBC How to Code: Simple Data](https://www.edx.org/course/how-code-simple-data-ubcx-htc1x)   | `learn`   | 60 hours  |
| `course` | [UBC How to Code: Complex Data](https://www.edx.org/course/how-code-complex-data-ubcx-htc2x) | `learn`   | 60 hours  |

### Imperative Computation
In Functional Computation, you learned how to compose very complex computations based on pure expressions, where all you needed were values (like integers) and functions that map variables to results.
However, there was one special construct, `define`, that behaved differently: it implicitly modified an "environment", making that binding available anywhere in that same scope without needing parentheses to create that scope.
This is in contrast to `let`, which *explicitly* put a binding into a scope: **the binding disappeared as soon as the last parenthesis of the `let` was closed.**
Thus, `define` was an example of a *statement*, and BSL/ISL used it because it's often syntactically more convenient than always using explicitly scoped `let` bindings.
(Thus, `define` can be thought of merely as syntactic sugar for a global `let` binding, so your programs were still a *single expression* containing many sub-expressions.)

In this section, you will learn a style called imperative programming, which is based on statements (or "commands").
Each statement modifies the environment after it's evaluated, just like BSL's `define`, but imperative languages have many more possible statements — most importantly, the notion of "assignment" (where the value inside a binding changes after evaluation of the statement).
Altogether, this ubiquitous mutation creates a whole host of complexities but is closer to how [von Neumann machines](https://en.wikipedia.org/wiki/Von_Neumann_architecture) operate at a low level, thus it is essential to learn how it works.

Choose either the book, which is not free, or the course, which should be free but may not always be accessible.

| Format   | Resource                                                                                             | Use cases | Length    |
|----------|------------------------------------------------------------------------------------------------------|-----------|-----------|
| `book`   | *[Think Java](https://books.trinket.io/thinkjava/)* (Allen Downey and Chris Mayfield)                | `learn`   | 252 pages |
| `course` | [MIT Software Construction in Java](https://www.edx.org/course/software-construction-java-mitx-6-005-1x) | `learn`   | 180 hours |

### Parallel Computation
So far you have learned how to program computers in a purely sequential manner and style.
But the reality is that computers nowadays have many threads and CPUs available, and it would be a colossal waste not to use them.
In this and the following section, you will learn the key concepts for scaling computations across multiple threads and cores of a single computer.
In Core Distributed Systems, you will then learn how to scale computation to multiple computers.

TODO: explain parallelism vs. concurrency

Choose at least the book or the course, but use both if you can.
Unfortunately, we are still looking for completely free of charge resources on this subject.

| Format          | Resource                                                                                                                                            | Use cases           | Length    |
|-----------------|-----------------------------------------------------------------------------------------------------------------------------------------------------|---------------------|-----------|
| `book`          | *[The Art of Multiprocessor Programming](https://www.amazon.com/Art-Multiprocessor-Programming-Revised-Reprint/dp/0123973376)* (Herlihy and Shavit) | `learn`             | 536 pages |
| `slides` `code` | [Companion Materials for *The Art of Multiprocessor Programming*](http://booksite.elsevier.com/9780123705914/?ISBN=9780123705914)                   | `review` `practice` |           |
| `course`        | [Parallel Programming in Java](https://www.coursera.org/learn/parallel-programming-in-java)                                                         | `learn`             | 48 hours  |

### Concurrent Computation
Choose the book or the course.
If you did the course in Parallel Computation, choose the course here as they are part of a set.

Unfortunately, we are still looking for completely free of charge resources on this subject.

| Format   | Resource                                                                                                                               | Use cases | Length    |
|----------|----------------------------------------------------------------------------------------------------------------------------------------|-----------|-----------|
| `book`   | *[Java Threads: Understanding and Mastering Concurrent Programming](http://shop.oreilly.com/product/9780596007829.do)* (Oaks and Wong) | `learn`   | 360 pages |
| `course` | [Concurrent Programming in Java](https://www.coursera.org/learn/concurrent-programming-in-java)                                        | `learn`   | 48 hours  |

## Needed by
- TODO