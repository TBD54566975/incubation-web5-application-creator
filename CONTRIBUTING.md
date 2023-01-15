# Contribution Guide 

There are many ways to be an open source contributor, and we're here to help you on your way! You may:

* Propose ideas in our 
  [discussion forums](https://forums.tbd.website)
* Raise an issue or feature request in our [issue tracker](https://github.com/TBD54566975/incubation-web5-application-creator/issues)
* Help another contributor with one of their questions, or a code review
* Suggest improvements to our Getting Started documentation by supplying a Pull Request
* Evangelize our work together in conferences, podcasts, and social media spaces.

This guide is for you.

## Development Prerequisites

___***UPDATE TABLE OF PROJECT DEPS AND INSTALLATION NOTES***___

| Requirement | Tested Version | Installation Instructions                            |
|-------------|----------------|------------------------------------------------------|
| Java        | 19.0.1         | Below, recommended via [SDKMan](https://sdkman.io)   |

### Java

This project is written in Java, a typesafe, compiled programming language. 

You may verify your `java` installation via the terminal by running `java -version`.

If you do not have Java, we recommend installing it 
via [SDKMan](https://sdkman.io/install). This is a project which will allow you 
to easily install the Java Development Kit (JDK), runtime (JRE), and related frameworks, 
build tools, and runtimes.

After you've installed SDKMan, you may install Java:

#### SDKMan (cross-platform instructions)

```shell
$> sdk install java 19.0.1-open
 ...
Do you want java 19.0.1-open to be set as default? (Y/n): Y
Setting java 19.0.1-open as default.
```

You may test your installation:

```shell
$> java -version
openjdk 19.0.1 2022-10-18
OpenJDK Runtime Environment (build 19.0.1+10-21)
OpenJDK 64-Bit Server VM (build 19.0.1+10-21, mixed mode, sharing)
```

---
**NOTE**

You may additionally look for other Java versions to install by running `sdk list java`:

...or other installation candidates like Apache Ant, Apache Maven, etc, by running `sdk list`.

Consult the SDKMan documentation for more info.

---

## Build (Java / Maven)

### macOS / Linux
```shell
$> ./mvn clean verify
```

## Test (Java / Maven)

### macOS / Linux
```shell
$> ./mvn test
```

---
**NOTE**

You may also combine Maven build targets in one call, like:

```shell
$> ./mvn test verify
```

---

## Communications

### Issues

Anyone from the community is welcome (and encouraged!) to raise issues via 
[GitHub Issues](https://github.com/TBD54566975/incubation-web5-application-creator/issues).

### Discussions

Design discussions and proposals take place on our [discussion forums](https://forums.tbd.website).

We advocate an asynchronous, written debate model - so write up your thoughts and invite the community to join in!

### Continuous Integration

TODO - Set up once build is active

## Contribution

We review contributions to the codebase via GitHub's Pull Request mechanism. We have 
the following guidelines to ease your experience and help our leads respond quickly 
to your valuable work:

* Start by proposing a change either in Issues (most appropriate for small 
  change requests or bug fixes) or in Discussions (most appropriate for design 
  and architecture considerations, proposing a new feature, or where you'd 
  like insight and feedback)
* Cultivate consensus around your ideas; the project leads will help you 
  pre-flight how beneficial the proposal might be to the project. Developing early 
  buy-in will help others understand what you're looking to do, and give you a 
  greater chance of your contributions making it into the codebase! No one wants to 
  see work done in an area that's unlikely to be incorporated into the codebase.
* Fork the repo into your own namespace/remote
* Work in a dedicated feature branch. Atlassian wrote a great 
  [description of this workflow](https://www.atlassian.com/git/tutorials/comparing-workflows/feature-branch-workflow)
* When you're ready to offer your work to the project, first:
* Squash your commits into a single one (or an appropriate small number of commits), and 
  rebase atop the upstream `main` branch. This will limit the potential for merge 
  conflicts during review, and helps keep the audit trail clean. A good writeup for 
  how this is done is 
  [here](https://medium.com/@slamflipstrom/a-beginners-guide-to-squashing-commits-with-git-rebase-8185cf6e62ec), and if you're 
  having trouble - feel free to ask a member or the community for help or leave the commits as-is, and flag that you'd like 
  rebasing assistance in your PR! We're here to support you.
* Open a PR in the project to bring in the code from your feature branch.
* The maintainers noted in the `CODEOWNERS` file will review your PR and optionally 
  open a discussion about its contents before moving forward.
* Remain responsive to follow-up questions, be open to making requested changes, and...
  You're a contributor!
* And remember to respect everyone in our global development community. Guidelines 
  are established in our `CODE_OF_CONDUCT.md`.