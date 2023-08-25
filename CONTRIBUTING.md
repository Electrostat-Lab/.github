# Contributing

> These rules apply to all the repositories produced by this organization, and the active external forks ONLY.

This guide will be an abstract guide that should work for any repository here.

## Table of contents: 
* General Contributions Rules.
* Discussions.
* Coding Styles (Java, C/C++ and Bash).
* Example of an OSS contribution.
* How to write a good issue description.
* How to write a good PR.

### General Contributions Rules
* Open an issue to discuss your feature or point out your bug before working on it,
Opening issues is a perfect way to keep track of the history of your work.
* Fork and clone your fork locally.
* Check out to a new branch and start working on the discussed changes.
* Follow the coding styles found in the appendix of this guide. Keep it simple and stupid, but not simpler!
* Your PR should illustrate exactly what you did to each change you proposed.
* Newly proposed APIs must be documented in the same PR.
* Any new feature should have at least one example illustrating how the API is utilized in a full application environment (**not unit testing**).
* Unit testing has minimal usage across the repositories here (since it's not a real application).
* Features or stress tests utilizing a native API should be tested on all the supported platforms before merging the PR.

## Discussions 
Discussions about bugs, design defects, and features can be instantiated in different ways: 
* The repositories' discussions.
* The repositories' issues.
> It's highly recommended to open an issue for the bug you found or the feature you want to add.

### Coding Styles 
The repositories follow the following coding styles: 
* For **Java**, the coding style follows [Google Style of code](https://google.github.io/styleguide/javaguide.html).
* For **C/C++**, the coding style follows [NASA's Style of code](https://ntrs.nasa.gov/citations/19950022400) and [GNU libc style](https://www.gnu.org/prep/standards/standards.html).
* For **Bash**, there are no rules to follow specifically.

## Example of an OSS contribution
In [Automata4j](https://github.com/Software-Hardware-Codesign/Automata4j), recall we want to introduce the `DeterministicManager` for implementing the API for the deterministic finite-state-automata, the following steps should be followed: 
* Forking the repository, and cloning the fork.
> ```bash
> $ git clone https://github.com/_foo-organization_/Automata4j.git
> $ cd ./Automata4j
> ```
* Check out to a new featured branch.
> ```bash
> $ git checkout master -b featured-branch
> ```
* Do your changes to the API.
* Commit your changes individually for each file, and push them to your fork.
> ```bash
> $ git add ./Automata4j/automata4j/src/java/main/com/avrsandbox/core/deterministic
> $ git commit -m 'automata4j-core: introduced the deterministic pattern'
> $ git add ./Automata4j/automata4j/src/java/main/com/avrsandbox/util
> $ git commit -m 'automata4j-util: introduced an DFSA helper utility'
> $ git push origin featured-branch
> ```

## How to write a good issue description
* If the issue involves multiple tasks, it is best written using checkboxes to identify the to-do tasks.
* In general, issues should simply describe the problem, how to reproduce it in an application environment, a proposed solution for this problem (if known by the issuer), and why this solution is better than others.

This is a template for an issue on Automata4j: 
> * Title: [Core] Provide a template method to retrieve the TransitionalManager in an AutoState
> * Body: Provide a template method AutoState#getTransitionalManager().
> * Further comments: Well, it's better to provide a parameter of type TransitionalManager in AutoState methods.

## How to write a good PR
* Writing a good PR is never easy, describing what this PR targets (which issue), what this PR has added, and how to test this PR is required.
* If the PR has added/modified multiple files, describing each addition/modification is also necessary.
* Training yourself on good practices from the start will help you boost your Open Source Skills.
* Here is [a good example of a tasked PR](https://github.com/Software-Hardware-Codesign/Automata4j/pull/2) of introducing the Deterministic Finite-State-Automata (DFSA) pattern to the Automata4j framework: 

![image](https://github.com/Software-Hardware-Codesign/.github/assets/60224159/a71fda44-4bcd-4155-947a-53fdc5d4799e)


> Don't hesitate to directly message me if in doubt.
