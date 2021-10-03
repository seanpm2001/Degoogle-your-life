
***

# Google Golang

![https://github.com/seanpm2001/Degoogle-your-life/blob/main/Graphics/Google-Golang/Logo/Go_Logo_Blue.svg](https://github.com/seanpm2001/Degoogle-your-life/blob/main/Graphics/Google-Golang/Logo/Go_Logo_Blue.svg)

[Not to be confused with Go! (the original programming language before Google stole the name)](https://github.com/seanpm2001/Degoogle-your-life/wiki/Go!-programming-language/)

Go is a statically typed, compiled programming language designed at Google by Robert Griesemer, Rob Pike, and Ken Thompson. Go is syntactically similar to C, but with memory safety, garbage collection, structural typing, and CSP-style concurrency. The language is often referred to as Golang because of its domain name, golang.org, but the proper name is Go.

There are two major implementations:

Google's self-hosting "gc" compiler toolchain targeting multiple operating systems, and WebAssembly.

gofrontend, a frontend to other compilers, with the libgo library. With GCC the combination is gccgo; with LLVM the combination is gollvm.

A third-party source-to-source compiler, GopherJS, compiles Go to JavaScript for front-end web development.

## History

Go was designed at Google in 2007 to improve programming productivity in an era of multicore, networked machines and large codebases. The designers wanted to address criticism of other languages in use at Google, but keep their useful characteristics:

static typing and run-time efficiency (like C),

readability and usability (like Python or JavaScript),

high-performance networking and multiprocessing.

The designers were primarily motivated by their shared dislike of C++.

Go was publicly announced in November 2009, and version 1.0 was released in March 2012. Go is widely used in production at Google and in many other organizations and open-source projects.

![https://github.com/seanpm2001/Degoogle-your-life/blob/main/Graphics/Google-Golang/Gopher/Golang.png](https://github.com/seanpm2001/Degoogle-your-life/blob/main/Graphics/Google-Golang/Gopher/Golang.png)

Mascot of Go programming language is a Gopher shown above.

In November 2016, the Go and Go Mono fonts were released by type designers Charles Bigelow and Kris Holmes specifically for use by the Go project. Go is a humanist sans-serif which resembles Lucida Grande and Go Mono is monospaced. Each of the fonts adhere to the WGL4 character set and were designed to be legible with a large x-height and distinct letterforms. Both Go and Go Mono adhere to the DIN 1450 standard by having a slashed zero, lowercase l with a tail, and an uppercase I with serifs.

In April 2018, the original logo was replaced with a stylized GO slanting right with trailing streamlines. However, the Gopher mascot remained the same.

In August 2018, the Go principal contributors published two "draft designs" for new and incompatible "Go 2" language features, generics and error handling, and asked Go users to submit feedback on them. Lack of support for generic programming and the verbosity of error handling in Go 1.x had drawn considerable criticism.

## Version history

Go 1 guarantees compatibility for the language specification and major parts of the standard library. All versions up to the current Go 1.17 release have maintained this promise.

Each major Go release is supported until there are two newer major releases.

Version history of Go Major version 	Initial release date 	Language changes 	Other changes

1–1.0.3 	2012-03-28 	Initial release 	

1.1–1.1.2 	2013-05-13 	

In Go 1.1, an integer division by constant zero is not a legal program, so it is a compile-time error.

The definition of string and rune literals has been refined to exclude surrogate halves from the set of valid Unicode code points.

Loosened return requirements rules. If the compiler can prove that a function always returns before reaching the end of a function, a final terminating statement can be omitted.	

The language allows the implementation to choose whether the int type and uint types are 32 or 64 bits.

On 64-bit architectures, the maximum heap size has been enlarged substantially, from a few gigabytes to several tens of gigabytes.

Addition of a race detector to the standard tool set.

1.2–1.2.2 	2013-12-01 	

The language now specifies that, for safety reasons, certain uses of nil pointers are guaranteed to trigger a run-time panic.
Go 1.2 adds the ability to specify the capacity as well as the length when using a slicing operation on an existing array or slice. A slicing operation creates a new slice by describing a contiguous section of an already-created array or slice.

The runtime scheduler can now be invoked on (non-inlined) function calls.

Go 1.2 introduces a configurable limit (default 10,000) to the total number of threads a single program may have.

In Go 1.2, the minimum size of the stack when a goroutine is created has been lifted from 4KB to 8KB.

1.3–1.3.3 	2014-06-18 	There are no language changes in this release. 	

The Go 1.3 memory model adds a new rule concerning sending and receiving on buffered channels, to make explicit that a buffered channel can be used as a simple semaphore, using a send into the channel to acquire and a receive from the channel to release.

Go 1.3 has changed the implementation of goroutine stacks away from the old, "segmented" model to a contiguous model.

For a while now, the garbage collector has been precise when examining values in the heap; the Go 1.3 release adds equivalent precision to values on the stack.

Iterations over small maps no longer happen in a consistent order. This is due to developers abusing implementation behaviour.

1.4–1.4.3 	2014-12-10 	

Range-expression without assignment

Automatic double-dereference on method calls is now disallowed in gc and gccgo. This is a backwards incompatible change, but in line with the language specification.

In 1.4, much of the runtime code has been translated to Go so that the garbage collector can scan the stacks of programs in the runtime and get accurate information about what variables are active.

The language accepted by the assemblers cmd/5a, cmd/6a and cmd/8a has had several changes, mostly to make it easier to deliver type information to the runtime.

Addition of internal packages.

New subcommand go generate.

1.5–1.5.4 	2015-08-19 	

Due to an oversight, the rule that allowed the element type to be elided from slice literals was not applied to map keys. This has been corrected in Go 1.5.

The compiler and runtime are now implemented in Go and assembler, without C. Now that the Go compiler and runtime are implemented in Go, a Go compiler must be available to compile the distribution from source. The compiler is now self-hosted.

The garbage collector has been re-engineered for 1.5. The "stop the world" phase of the collector will almost always be under 10 milliseconds and usually much less.

In Go 1.5, the order in which goroutines are scheduled has been changed.

1.6–1.6.4 	2016-02-17 	There are no language changes in this release. 	

A major change was made to cgo defining the rules for sharing Go pointers with C code, to ensure that such C code can coexist with Go's garbage collector.

The Go parser is now hand-written instead of generated.

The go vet command now diagnoses passing function or method values as arguments to Printf, such as when passing f where f() was intended.

1.7–1.7.6 	2016-08-15 	

Clarification on terminating statements in the language specification. This does not change existing behaviour.	

For 64-bit x86 systems, the following instructions have been added (see SSE): PCMPESTRI, RORXL, RORXQ, VINSERTI128, VPADDD, VPADDQ, VPALIGNR, VPBLENDD, VPERM2F128, VPERM2I128, VPOR, VPSHUFB, VPSHUFD, VPSLLD, VPSLLDQ, VPSLLQ, VPSRLD, VPSRLDQ, and VPSRLQ .

This release includes a new code generation back end for 64-bit x86 systems, based on SSA.

Packages using cgo may now include Fortran source files (in addition to C, C++, Objective C, and SWIG), although the Go bindings must still use C language APIs.

The new subcommand "go tool dist list" prints all supported operating system/architecture pairs.

1.8–1.8.7 	2017-02-16 	

When explicitly converting a value from one struct type to another, as of Go 1.8 the tags are ignored. Thus two structs that differ only in their tags may be converted from one to the other.

For 64-bit x86 systems, the following instructions have been added: VBROADCASTSD, BROADCASTSS, MOVDDUP, MOVSHDUP, MOVSLDUP, VMOVDDUP, VMOVSHDUP, and VMOVSLDUP.

Garbage collection pauses should be significantly shorter than they were in Go 1.7, usually under 100 microseconds and often as low as 10 microseconds. See the document on eliminating stop-the-world stack re-scanning for details.

The overhead of deferred function calls has been reduced by about half.

The overhead of calls from Go into C has been reduced by about half.

1.9–1.9.7 	2017-08-24 	

Go now supports type aliases.

Force the intermediate rounding in floating-point arithmetic.

The Go compiler now supports compiling a package's functions in parallel, taking advantage of multiple cores.

1.10–1.10.7 	2018-02-16 	

A corner case involving shifts of untyped constants has been clarified.

The grammar for method expressions has been updated to relax the syntax to allow any type expression as a receiver.

For the x86 64-bit port, the assembler now supports 359 new instructions, including the full AVX, AVX2, BMI, BMI2, F16C, FMA3, SSE2, SSE3, SSSE3, SSE4.1, and SSE4.2 extension sets. The assembler also no longer implements MOVL $0, AX as an XORL instruction, to avoid clearing the condition flags unexpectedly.

1.11–1.11.6 	2018-08-24 	There are no language changes in this release. 	

Go 1.11 adds an experimental port to WebAssembly.

Go 1.11 adds preliminary support for a new concept called "modules", an alternative to GOPATH with integrated support for versioning and package distribution.

The assembler for amd64 now accepts AVX512 instructions.

Go 1.11 drops support of Windows XP and Windows Vista.

Go 1.11.3 and later fix the TLS authentication vulnerability in the crypto/x509 package.

1.12.1 	2019-02-25 	There are no language changes in this release. 	

Opt-in support for TLS 1.3

Improved modules support (in preparation for being the default in Go 1.13)

Support for windows/arm

Improved macOS & iOS forwards compatibility

1.13.1 	2019-09-03 	

Go now supports a more uniform and modernized set of number literal prefixes

support for TLS 1.3 in the crypto/tls package by default (opt-out will be removed in Go 1.14)
Support for error wrapping

1.14 	2020-02-25 	

Permits embedding interfaces with overlapping method sets

Module support in the go command is now ready for production use
1.15 	2020-08-11 	There are no language changes in this release. 	

New embedded time/tzdata package

The printing verbs %#g and %#G now preserve trailing zeros for floating-point values

Package reflect now disallows accessing methods of all non-exported fields, whereas previously it allowed accessing those of non-exported, embedded fields.

1.16 	2021-02-16 	There are no language changes in this release. 	

New support for embedding files inside a go program

Support for macos/arm

Module-aware mode is enabled by default

1.17 	2021-08-16 	There are no language changes in this release. 	

This update primarily modifies Go internals

## Design

Go is influenced by C (especially the Plan 9 dialect), but with an emphasis on greater simplicity and safety. The language consists of:

A syntax and environment adopting patterns more common in dynamic languages:

Optional concise variable declaration and initialization through type inference (x := 0 instead of int x = 0; or var x = 0;).

Fast compilation.

Remote package management (go get) and online package documentation.

Distinctive approaches to particular problems:

Built-in concurrency primitives: light-weight processes (goroutines), channels, and the select statement.

An interface system in place of virtual inheritance, and type embedding instead of non-virtual inheritance.

A toolchain that, by default, produces statically linked native binaries without external dependencies.

A desire to keep the language specification simple enough to hold in a programmer's head, in part by omitting features that are common in similar languages.

## Syntax

Go's syntax includes changes from C aimed at keeping code concise and readable. A combined declaration/initialization operator was introduced that allows the programmer to write i := 3 or s := "Hello, world!", without specifying the types of variables used. This contrasts with C's int i = 3; and const char *s = "Hello, world!";. Semicolons still terminate statements,[b] but are implicit when the end of a line occurs. Methods may return multiple values, and returning a result, err pair is the conventional way a method indicates an error to its caller in Go. Go adds literal syntaxes for initializing struct parameters by name and for initializing maps and slices. As an alternative to C's three-statement for loop, Go's range expressions allow concise iteration over arrays, slices, strings, maps, and channels.

### Types

Go has a number of built-in types, including numeric ones (byte, int64, float32, etc.), booleans, and character strings (string). Strings are immutable; built-in operators and keywords (rather than functions) provide concatenation, comparison, and UTF-8 encoding/decoding. Record types can be defined with the struct keyword.

For each type T and each non-negative integer constant n, there is an array type denoted T; arrays of differing lengths are thus of different types. Dynamic arrays are available as "slices", denoted []T for some type T. These have a length and a capacity specifying when new memory needs to be allocated to expand the array. Several slices may share their underlying memory.

Pointers are available for all types, and the pointer-to-T type is denoted *T. Address-taking and indirection use the & and * operators, as in C, or happen implicitly through the method call or attribute access syntax. There is no pointer arithmetic, except via the special unsafe.Pointer type in the standard library.

For a pair of types K, V, the type map[K]V is the type of hash tables mapping type-K keys to type-V values. Hash tables are built into the language, with special syntax and built-in functions. chan T is a channel that allows sending values of type T between concurrent Go processes.

Aside from its support for interfaces, Go's type system is nominal: the type keyword can be used to define a new named type, which is distinct from other named types that have the same layout (in the case of a struct, the same members in the same order). Some conversions between types (e.g., between the various integer types) are pre-defined and adding a new type may define additional conversions, but conversions between named types must always be invoked explicitly. For example, the type keyword can be used to define a type for IPv4 addresses, based on 32-bit unsigned integers:

```go
type ipv4addr uint32
```

With this type definition, ipv4addr(x) interprets the uint32 value x as an IP address. Simply assigning x to a variable of type ipv4addr is a type error.

Constant expressions may be either typed or "untyped"; they are given a type when assigned to a typed variable if the value they represent passes a compile-time check.

Function types are indicated by the func keyword; they take zero or more parameters and return zero or more values, all of which are typed. The parameter and return values determine a function type; thus, func(string, int32) (int, error) is the type of functions that take a string and a 32-bit signed integer, and return a signed integer (of default width) and a value of the built-in interface type error.

Any named type has a method set associated with it. The IP address example above can be extended with a method for checking whether its value is a known standard:

```go
// ZeroBroadcast reports whether addr is 255.255.255.255.
func (addr ipv4addr) ZeroBroadcast() bool {
return addr == 0xFFFFFFFF
}
```

Due to nominal typing, this method definition adds a method to ipv4addr, but not on uint32. While methods have special definition and call syntax, there is no distinct method type.

### Interface system

Go provides two features that replace class inheritance.

The first is embedding, which can be viewed as an automated form of composition or delegation.

The second are its interfaces, which provides runtime polymorphism.  Interfaces are a class of types and provide a limited form of structural typing in the otherwise nominal type system of Go. An object which is of an interface type is also of another type, much like C++ objects being simultaneously of a base and derived class. Go interfaces were designed after protocols from the Smalltalk programming language. Multiple sources use the term duck typing when describing Go interfaces. Although the term duck typing is not precisely defined and therefore not wrong, it usually implies that type conformance is not statically checked. Since conformance to a Go interface is checked statically by the Go compiler (except when performing a type assertion), the Go authors prefer the term structural typing.

The definition of an interface type lists required methods by name and type. Any object of type T for which functions exist matching all the required methods of interface type I is an object of type I as well. The definition of type T need not (and cannot) identify type I. For example, if Shape, Square and Circle are defined as

```go
import "math"

type Shape interface {
Area() float64
}

type Square struct { // Note: no "implements" declaration
side float64
}

func (sq Square) Area() float64 { return sq.side * sq.side }

type Circle struct { // No "implements" declaration here either
radius float64
}

func (c Circle) Area() float64 { return math.Pi * math.Pow(c.radius, 2) }
```

then both a Square and a Circle are implicitly a Shape and can be assigned to a Shape-typed variable.  In formal language, Go's interface system provides structural rather than nominal typing. Interfaces can embed other interfaces with the effect of creating a combined interface that is satisfied by exactly the types that implement the embedded interface and any methods that the newly defined interface adds.

The Go standard library uses interfaces to provide genericity in several places, including the input/output system that is based on the concepts of Reader and Writer.

Besides calling methods via interfaces, Go allows converting interface values to other types with a run-time type check. The language constructs to do so are the type assertion, which checks against a single potential type, and the type switch, which checks against multiple types.

The empty interface interface{} is an important base case because it can refer to an item of any concrete type. It is similar to the Object class in Java or C# and is satisfied by any type, including built-in types like int.  Code using the empty interface cannot simply call methods (or built-in operators) on the referred-to object, but it can store the interface{} value, try to convert it to a more useful type via a type assertion or type switch, or inspect it with Go's reflect package. Because interface{} can refer to any value, it is a limited way to escape the restrictions of static typing, like void* in C but with additional run-time type checks.

The interface{} type can be used to model structured data of any arbitrary schema in Go, such as JSON or YAML data, by representing it as a map[string]interface{} (map of string to empty interface). This recursively describes data in the form of a dictionary with string keys and values of any type.

Interface values are implemented using pointer to data and a second pointer to run-time type information/. Like some other types implemented using pointers in Go, interface values are nil if uninitialized.

### Package system

In Go's package system, each package has a path (e.g., "compress/bzip2" or "golang.org/x/net/html") and a name (e.g., bzip2 or html). References to other packages' definitions must always be prefixed with the other package's name, and only the capitalized names from other packages are accessible: io.Reader is public but bzip2.reader is not. The go get command can retrieve packages stored in a remote repository[80] and developers are encouraged to develop packages inside a base path corresponding to a source repository (such as example.com/user_name/package_name) to reduce the likelihood of name collision with future additions to the standard library or other external libraries.[

Proposals exist to introduce a proper package management solution for Go similar to CPAN for Perl or Rust's cargo system or Node's npm system.

### Concurrency: goroutines and channels

The Go language has built-in facilities, as well as library support, for writing concurrent programs. Concurrency refers not only to CPU parallelism, but also to asynchrony: letting slow operations like a database or network read run while the program does other work, as is common in event-based servers.

The primary concurrency construct is the goroutine, a type of light-weight process. A function call prefixed with the go keyword starts a function in a new goroutine. The language specification does not specify how goroutines should be implemented, but current implementations multiplex a Go process's goroutines onto a smaller set of operating-system threads, similar to the scheduling performed in Erlang.

While a standard library package featuring most of the classical concurrency control structures (mutex locks, etc.) is available,  idiomatic concurrent programs instead prefer channels, which provide send messages between goroutines. Optional buffers store messages in FIFO order and allow sending goroutines to proceed before their messages are received.

Channels are typed, so that a channel of type chan T can only be used to transfer messages of type T. Special syntax is used to operate on them; <-ch is an expression that causes the executing goroutine to block until a value comes in over the channel ch, while ch <- x sends the value x (possibly blocking until another goroutine receives the value). The built-in switch-like select statement can be used to implement non-blocking communication on multiple channels; see below for an example. Go has a memory model describing how goroutines must use channels or other operations to safely share data.

The existence of channels sets Go apart from actor model-style concurrent languages like Erlang, where messages are addressed directly to actors (corresponding to goroutines). The actor style can be simulated in Go by maintaining a one-to-one correspondence between goroutines and channels, but the language allows multiple goroutines to share a channel or a single goroutine to send and receive on multiple channels.

From these tools one can build concurrent constructs like worker pools, pipelines (in which, say, a file is decompressed and parsed as it downloads), background calls with timeout, "fan-out" parallel calls to a set of services, and others. Channels have also found uses further from the usual notion of interprocess communication, like serving as a concurrency-safe list of recycled buffers, implementing coroutines (which helped inspire the name goroutine), and implementing iterators.

Concurrency-related structural conventions of Go (channels and alternative channel inputs) are derived from Tony Hoare's communicating sequential processes model. Unlike previous concurrent programming languages such as Occam or Limbo (a language on which Go co-designer Rob Pike worked), Go does not provide any built-in notion of safe or verifiable concurrency. While the communicating-processes model is favored in Go, it is not the only one: all goroutines in a program share a single address space. This means that mutable objects and pointers can be shared between goroutines; see § Lack of race condition safety, below.

### Suitability for parallel programming

Although Go's concurrency features are not aimed primarily at parallel processing, they can be used to program shared-memory multi-processor machines. Various studies have been done into the effectiveness of this approach. One of these studies compared the size (in lines of code) and speed of programs written by a seasoned programmer not familiar with the language and corrections to these programs by a Go expert (from Google's development team), doing the same for Chapel, Cilk and Intel TBB. The study found that the non-expert tended to write divide-and-conquer algorithms with one go statement per recursion, while the expert wrote distribute-work-synchronize programs using one goroutine per processor. The expert's programs were usually faster, but also longer.
Lack of race condition safety

There are no restrictions on how goroutines access shared data, making race conditions possible. Specifically, unless a program explicitly synchronizes via channels or other means, writes from one goroutine might be partly, entirely, or not at all visible to another, often with no guarantees about ordering of writes. Furthermore, Go's internal data structures like interface values, slice headers, hash tables, and string headers are not immune to race conditions, so type and memory safety can be violated in multithreaded programs that modify shared instances of those types without synchronization. Instead of language support, safe concurrent programming thus relies on conventions; for example, Chisnall recommends an idiom called "aliases xor mutable", meaning that passing a mutable value (or pointer) over a channel signals a transfer of ownership over the value to its receiver.

### Binaries

The linker in the gc toolchain creates statically linked binaries by default; therefore all Go binaries include the Go runtime.

### Omissions

Go deliberately omits certain features common in other languages, including (implementation) inheritance, generic programming, assertions, pointer arithmetic, implicit type conversions, untagged unions, and tagged unions. The designers added only those facilities that all three agreed on.

Of the omitted language features, the designers explicitly argue against assertions and pointer arithmetic, while defending the choice to omit type inheritance as giving a more useful language, encouraging instead the use of interfaces to achieve dynamic dispatch and composition to reuse code. Composition and delegation are in fact largely automated by struct embedding; according to researchers Schmager et al., this feature "has many of the drawbacks of inheritance: it affects the public interface of objects, it is not fine-grained (i.e, no method-level control over embedding), methods of embedded objects cannot be hidden, and it is static", making it "not obvious" whether programmers will overuse it to the extent that programmers in other languages are reputed to overuse inheritance.

The designers express an openness to generic programming and note that built-in functions are in fact type-generic, but these are treated as special cases; Pike calls this a weakness that may at some point be changed. The Google team built at least one compiler for an experimental Go dialect with generics, but did not release it. They are also open to standardizing ways to apply code generation. In June 2020, a new draft design document was published, which would add the necessary syntax to Go for declaring generic functions and types. A code translation tool go2go was provided to allow users to try out the new syntax, along with a generics-enabled version of the online Go Playground.

Initially omitted, the exception-like panic/recover mechanism was eventually added, which the Go authors advise using for unrecoverable errors such as those that should halt an entire program or server request, or as a shortcut to propagate errors up the stack within a package (but not across package boundaries; there, error returns are the standard API).

### Style
	
This section possibly contains original research. Please improve it by verifying the claims made and adding inline citations. Statements consisting only of original research should be removed. (January 2018) (Learn how and when to remove this template message)

The Go authors put substantial effort into influencing the style of Go programs:

Indentation, spacing, and other surface-level details of code are automatically standardized by the gofmt tool. golint does additional style checks automatically.

Tools and libraries distributed with Go suggest standard approaches to things like API documentation (godoc), testing (go test), building (go build), package management (go get), and so on.

Go enforces rules that are recommendations in other languages, for example banning cyclic dependencies, unused variables or imports, and implicit type conversions.

The omission of certain features (for example, functional-programming shortcuts like map and Java-style try/finally blocks) tends to encourage a particular explicit, concrete, and imperative programming style.

On day one the Go team published a collection of Go idioms, and later also collected code review comments, talks, and official blog posts to teach Go style and coding philosophy.

### Tools

The main Go distribution includes tools for building, testing, and analyzing code:

go build, which builds Go binaries using only information in the source files themselves, no separate makefiles

go test, for unit testing and microbenchmarks

go fmt, for formatting code

go install, for retrieving and installing remote packages

go vet, a static analyzer looking for potential errors in code

go run, a shortcut for building and executing code

godoc, for displaying documentation or serving it via HTTP

gorename, for renaming variables, functions, and so on in a type-safe way

go generate, a standard way to invoke code generators

It also includes profiling and debugging support, runtime instrumentation (for example, to track garbage collection pauses), and a race condition tester.

An ecosystem of third-party tools adds to the standard distribution, such as gocode, which enables code autocompletion in many text editors, goimports, which automatically adds/removes package imports as needed, and errcheck, which detects code that might unintentionally ignore errors.

## Examples

### Hello world

```go
package main

import "fmt"

func main() {
fmt.Println("Hello, world!")
}
```

where "fmt" is the package for formatted I/O, similar to C's C file input/output.[

### Concurrency

The following simple program demonstrates Go's concurrency features to implement an asynchronous program. It launches two lightweight threads ("goroutines"): one waits for the user to type some text, while the other implements a timeout. The select statement waits for either of these goroutines to send a message to the main routine, and acts on the first message to arrive (example adapted from David Chisnall's book)

```go
package main

import (
"fmt"
"time"
)

func readword(ch chan string) {
fmt.Println("Type a word, then hit Enter.")
var word string
fmt.Scanf("%s", &word)
ch <- word
}

func timeout(t chan bool) {
time.Sleep(5 * time.Second)
t <- false
}

func main() {
t := make(chan bool)
go timeout(t)

ch := make(chan string)
go readword(ch)

select {
case word := <-ch:
fmt.Println("Received", word)
case <-t:
fmt.Println("Timeout.")
}
}
```

### Testing

The testing package provides support for automated testing of go packages. Target function example:

```go
func ExtractUsername(email string) string {
	at := strings.Index(email, "@")
	return email[:at]
}
```

Test code (note that assert keyword is missing in Go; tests live in <filename>_test.go at the same package):

```go
import (
"testing"
)

func TestExtractUsername(t *testing.T) {
	t.Run("withoutDot", func(t *testing.T) {
		username := ExtractUsername("r@google.com")
		if username != "r" {
			t.Fatalf("Got: %v\n", username)
		}
	})

	t.Run("withDot", func(t *testing.T) {
		username := ExtractUsername("jonh.smith@example.com")
		if username != "jonh.smith" {
			t.Fatalf("Got: %v\n", username)
		}
	})

}
```

It is possible to run tests in parallel.

###Web App

The net/http package provides support for creating web applications.

This example would show "Hello world!" when localhost:8080 is visited.

```go
package main

import (
"fmt"
"log"
"net/http"
)

func helloFunc(w http.ResponseWriter, r *http.Request) {
fmt.Fprintf(w, "Hello world!")
}

func main() {
http.HandleFunc("/", helloFunc)
log.Fatal(http.ListenAndServe(":8080", nil))
}
```

## Applications

Some notable open-source applications written in Go include:

Caddy, an open source HTTP/2 web server with automatic HTTPS capability

CockroachDB, an open source, survivable, strongly consistent, scale-out SQL database

Consul, a software for DNS-based service discovery and providing distributed Key-value storage, segmentation and configuration.

Docker, a set of tools for deploying Linux containers

EdgeX, a vendor-neutral open-source platform hosted by the Linux Foundation, providing a common framework for industrial IoT edge computing

Hugo, a static site generator

InfluxDB, an open source database specifically to handle time series data with high availability and high performance requirements

InterPlanetary File System, a content-addressable, peer-to-peer hypermedia protocol

Juju, a service orchestration tool by Canonical, packagers of Ubuntu Linux

Kubernetes container management system

lnd, an implementation of the Bitcoin Lightning Network

Mattermost, a teamchat system

NATS Messaging, an open-source messaging system featuring the core design principles of performance, scalability, and ease of use

OpenShift, a cloud computing platform as a service by Red Hat

Rclone, a command line program to manage files on cloud storage and other high latency services

Snappy, a package manager for Ubuntu Touch developed by Canonical

Syncthing, an open-source file synchronization client/server application

Terraform, an open-source, multiple cloud infrastructure provisioning tool from HashiCorp

TiDB, an open-source, distributed HTAP database compatible with the MySQL protocol from PingCAP

Other notable companies and sites using Go (generally together with other languages, not exclusively) include:

Cacoo, for their rendering of the user dashboard page and microservice using Go and gRPC

Chango, a programmatic advertising company uses Go in its real-time bidding systems

Cloud Foundry, a platform as a service

Cloudflare, for their delta-coding proxy Railgun, their distributed DNS service, as well as tools for cryptography, logging, stream processing, and accessing SPDY sites

Container Linux (formerly CoreOS), a Linux-based operating system that uses Docker containers and rkt containers

Couchbase, Query and Indexing services within the Couchbase Server

Dropbox, who migrated some of their critical components from Python to Go

Ethereum, The go-ethereum implementation of the Ethereum Virtual Machine blockchain for the Ether cryptocurrency

Gitlab, a web-based DevOps lifecycle tool that provides a Git-repository, wiki, issue-tracking, continuous integration, deployment pipeline features

Google, for many projects, notably including download server dl.google.com.

Heroku, for Doozer, a lock service

Hyperledger Fabric, an open source, enterprise-focused distributed ledger project

MongoDB, tools for administering MongoDB instances

Netflix, for two portions of their server architecture

Nutanix, for a variety of micro-services in its Enterprise Cloud OS

Plug.dj, an interactive online social music streaming website[

SendGrid, a Boulder, Colorado-based transactional email delivery and management service.

SoundCloud, for "dozens of systems"

Splice, for the entire backend (API and parsers) of their online music collaboration platform

ThoughtWorks, some tools and applications for continuous delivery and instant messages (CoyIM)

Twitch, for their IRC-based chat system (migrated from Python)

Uber, for handling high volumes of geofence-based queries

## Reception

The interface system, and the deliberate omission of inheritance, were praised by Michele Simionato, who likened these characteristics to those of Standard ML, calling it "a shame that no popular language has followed [this] particular route".

Dave Astels at Engine Yard wrote:

Go is extremely easy to dive into. There are a minimal number of fundamental language concepts and the syntax is clean and designed to be clear and unambiguous. Go is still experimental and still a little rough around the edges.

Go was named Programming Language of the Year by the TIOBE Programming Community Index in its first year, 2009, for having a larger 12-month increase in popularity (in only 2 months, after its introduction in November) than any other language that year, and reached 13th place by January 2010, surpassing established languages like Pascal. By June 2015, its ranking had dropped to below 50th in the index, placing it lower than COBOL and Fortran. But as of January 2017, its ranking had surged to 13th, indicating significant growth in popularity and adoption. Go was awarded TIOBE programming language of the year 2016.

Bruce Eckel has stated:

The complexity of C++ (even more complexity has been added in the new C++), and the resulting impact on productivity, is no longer justified. All the hoops that the C++ programmer had to jump through in order to use a C-compatible language make no sense anymore -- they're just a waste of time and effort. Go makes much more sense for the class of problems that C++ was originally intended to solve.

A 2011 evaluation of the language and its gc implementation in comparison to C++ (GCC), Java and Scala by a Google engineer found:

Go offers interesting language features, which also allow for a concise and standardized notation. The compilers for this language are still immature, which reflects in both performance and binary sizes.
— R. Hundt

The evaluation got a rebuttal from the Go development team. Ian Lance Taylor, who had improved the Go code for Hundt's paper, had not been aware of the intention to publish his code, and says that his version was "never intended to be an example of idiomatic or efficient Go"; Russ Cox then optimized the Go code, as well as the C++ code, and got the Go code to run slightly faster than C++ and more than an order of magnitude faster than the code in the paper.

## Naming dispute

On November 10, 2009, the day of the general release of the language, Francis McCabe, developer of the Go! programming language (note the exclamation point), requested a name change of Google's language to prevent confusion with his language, which he had spent 10 years developing. McCabe raised concerns that "the 'big guy' will end up steam-rollering over" him, and this concern resonated with the more than 120 developers who commented on Google's official issues thread saying they should change the name, with some even saying the issue contradicts Google's motto of: Don't be evil.

On October 12, 2010, the issue was closed by Google developer Russ Cox (@rsc) with the custom status "Unfortunate" accompanied by the following comment:

"There are many computing products and services named Go. In the 11 months since our release, there has been minimal confusion of the two languages."

## Criticism

Go critics say that:

The lack of parametric polymorphism for generic programming leads to code duplication or unsafe type conversions and flow-disrupting verbosity.

Go's nil combined with the lack of algebraic types leads to difficulty handling failures and base cases.

Go does not allow an opening brace to appear on its own line, which forces all Go programmers to use the same brace style.

File semantics in Go standard library are heavily based on POSIX semantics, and they do not map well to the Windows platform. Note that this problem is not particular to Go, but other programming languages have solved it through well defined standard libraries. The author also argues that Go's simplicity is an illusion and that to solve real world problems, libraries with surprisingly large dependencies need to be pulled in to solve something as simple as implementing a monotonically increasing time function.

Study shows that it is as easy to make concurrency bugs with message passing as with shared memory, sometimes even more.

***

## Sources

[Go programming language on Wikipedia](https://en.wikipedia.org/wiki/Go_(programming_language))

I need more sources and better sources for this article. This article is also a stub, and needs to be expanded and rewritten in some parts.

***

## Article info

**Written on:** `2021 Saturday, October 2nd at 5:46 pm`

**Last revised on:** `2021 Saturday, October 2nd at 5:46 pm`

**File format** `Markdown document (*.md *.mkd *.markdown)`

**Line count (including blank lines and compiler line):** `682`

**Article version:** `1 (2021 Saturday, October 2nd at 5:46 pm)`

***

<!-- Tools

Quick copy and paste

https://github.com/seanpm2001/Degoogle-your-life/wiki/

!-->
