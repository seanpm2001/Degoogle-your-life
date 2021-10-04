
***

# Bazel

![https://github.com/seanpm2001/Degoogle-your-life/blob/main/Graphics/Bazel/Logo/2017/Bazel_logo.svg](https://github.com/seanpm2001/Degoogle-your-life/blob/main/Graphics/Bazel/Logo/2017/Bazel_logo.svg)

## Statistics

**Developer(s):**	Google

**Initial release:**	March 2015; 6 years ago

**Stable release:**	4.0.0 / 21 January 2021;

**Repository:** [github.com/bazelbuild/bazel](github.com/bazelbuild/bazel)

**Written in:**	Java

**Operating system:**	Cross-platform

**License:**	Apache License 2.0

**Website:**	[bazel.build](https://bazel.build)

Bazel is a free software tool for the automation of building and testing of software. The company Google uses the build tool Blaze internally and released an open-sourced part of the Blaze tool as Bazel, named as an anagram of Blaze. Bazel was first released in March 2015 and achieved beta status by September 2015.

Similar to build tools like Make, Apache Ant, or Apache Maven, Bazel builds software applications from source code using a set of rules. Rules and macros are created in the Starlark language (previously called Skylark), a dialect of Python. There are built-in rules for building software written in the programming languages of Java, C, C++, Go, Python, Objective-C and Bourne shell scripts. Bazel can produce software application packages suitable for deployment for the Android and iOS operating systems

## Rationale

One of the goals of Bazel is to create a build system where build target inputs and outputs are fully specified and therefore precisely known to the build system. This allows a more accurate analysis and determination of out-of-date build artifacts in the build system's dependency graph. Making the dependency graph analysis more deterministic leads to potential improvements in build times by avoiding re-executing unnecessary build targets. Build reliability is improved by avoiding errors where build targets might depend on out-of-date input artifacts.

To achieve more accurate dependency graph analysis, Bazel uses content digests rather than file-based timestamps. File timestamps are commonly used to detect changes in tools like Make or Apache Ant. Timestamps can be problematic when builds are distributed across multiple hosts due to issues with clock synchronization. One of Bazel's goals is to enable distributed and parallel builds on a remote cloud infrastructure. Bazel is also designed to scale up to very large build repositories which may not be practical to download to an individual developer's work machine.

Bazel provides tooling which helps developers to create bit-identical reproducible build outputs. Bazel's implemented rules avoid typical pitfalls such as embedding timestamps in generated outputs to ensure content digest matches. This in turn allows the build system to reliably cache (memoize) the outputs of intermediate build steps. Furthermore, reproducible build makes it possible to share intermediate build results between teams or departments in an organization, using dedicated build servers or distributed caches. Bazel therefore is particularly well-suited for larger organizations and software projects that have significant number of build dependencies. A deterministic build and an ability to precisely analyze build input and output artifacts across the dependency graph lends itself to parallel execution of build steps.

## Starlark language

Bazel is extensible with its custom Starlark programming language. Starlark uses a syntax which is a subset of the syntax of the Python programming language. Starlark however doesn't implement many of Python's language features, such as ability to mutate collections or access the file I/O, in order to avoid extensions that could create side-effects or create build outputs not known to the build system itself. Such side-effects could potentially lead to incorrect analysis of the build dependency graph.

Bazel was designed as a multi-language build system. Many commonly used build system are designed with a preference towards a specific programming language. Examples of such systems include Ant and Maven for Java, Leiningen for Clojure, sbt for Scala, etc. In a multi-language project, combining separate build systems and achieving the build speed and correctness benefits described above can be difficult and problematic.

Bazel also provides sand-boxed build execution. This can be used to ensure all build dependencies have been properly specified and the build does not depend, for example, on libraries installed only locally on a developer's work computer. This helps to ensure that builds remain portable and can be executed in other (remote) environments.

Build systems most similar to Bazel are Pants, Buck, and Please. Pants and Buck both aim for similar technical design goals as Bazel and were inspired by the Blaze build system used internally at Google. Blaze is also the predecessor to Bazel. Bazel, Pants, Buck, and Please adopted Starlark as BUILD file parser, respective its BUILD file syntax. Independently developed build systems with similar goals of efficient dependency graph analysis and automated build artifact tracking have been implemented in build systems such as tup.

## Sandbox

One of the key features that differentiate Bazel from other build systems is the use of a sandbox for compilation steps. When Bazel performs separate compilation, it creates a new directory and fills it with symlinks to the explicit input dependencies for the rule. For languages like C/C++, this provides a significant safety net for the inclusion of header files: it ensures that the developer is aware of the files that are used in compilation, and it prevents the unexpected inclusion of a similarly-named header file from another include directory.

This sandbox approach leads to issues with common build tools, resulting in a number of workarounds required to correctly compile code under different architectures. For example, when performing separate compilation for Mac/Darwin architectures, the compiler writes the input paths into SO and OSO symbols in the Mach-O binary, which can be seen with a command like nm -a mybinary | grep SO. These paths are needed for finding symbols during debugging. As a result, builds in Bazel must correct the compiled objects after the fact, trying to correct path-related issues that arose from the sandbox construction using flags like -fdebug-prefix-map and -oso_prefix, the latter having become available in XCode 11.0. Similar handling needs to take place in linking phases, rewriting the rpath values in shared object libraries with a command like install_name_tool.

## Logo

![https://github.com/seanpm2001/Degoogle-your-life/blob/main/Graphics/Bazel/Logo/First/Bazel_logo.png](https://github.com/seanpm2001/Degoogle-your-life/blob/main/Graphics/Bazel/Logo/First/Bazel_logo.png)

Since Bazel's initial release the logo was a green letter "b" stylized into a stem of a basil plant with two leaves.

On July 5, 2017, the Bazel Blog announced a new logo, consisting of three green building blocks arranged to shape a heart.

***

## Sources

![https://en.wikipedia.org/wiki/Android_(operating_system)](https://en.wikipedia.org/wiki/Android_(operating_system))

Other sources are needed, and this article needs LOTS of improvement and original work to prevent it from being partially copied from Wikipedia.

***

## Article info

**File type:** `Markdown document (*.md *.mkd *.markdown)`

**File version:** `1 (Sunday, 2021 October 3rd at 7:05 pm)`

**Line count (including blank lines and compiler line):** `89`

***

## Technical notes

**All times are UTC-7 (PDT/Pacific Time)**

**The encoding is UTF-8 and is compatible with Unicode 5.0 and up**

***
