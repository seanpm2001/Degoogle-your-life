
***

# Go! programming language

[Not to be confused with Go (the inappropriately named language by Google)](https://github.com/seanpm2001/Degoogle-your-life/wiki/Google-golang/)

Go! is an agent-based programming language in the tradition of logic-based programming languages like Prolog. It was introduced in a 2003 paper by Francis McCabe and Keith Clark.

## Design

The authors of Go! describe it as "a multi-paradigm programming language that is oriented to the needs of programming secure, production quality and agent-based applications. It is multi-threaded, strongly typed and higher order (in the functional programming sense). It has relation, function and action procedure definitions. Threads execute action procedures, calling functions and querying relations as needed. Threads in different agents communicate and coordinate using asynchronous messages. Threads within the same agent can also use shared dynamic relations acting as Linda-style tuple stores."

The authors also propose that the language is suitable for representing ontologies due to its integration of logic, functional and imperative styles of programming.

## Example

The following example illustrates the "ontology-oriented" type and declarations style of Go!:

```go
Sex ::= male | female.

person <~ {dayOfBirth:[] => day.
           age:[] => integer.
           sex:[] => Sex.
           name:[] => string.
           home:[] => string.
           lives:[string]{}}.
  
person:[string, day, Sex, string] $= person.
  
person(Nm, Born, Sx, Hm)..{
  dayOfBirth() => Born.
  age() => yearsBetween(now(), Born).
  sex() => Sx.
  name() => Nm.
  home() => Hm.
  lives(Pl) :- Pl = home().
  yearsBetween:[integer, day] => integer.
  yearsBetween(...) => ..
}.
  
newPerson:[string, day, Sex, string] => person.
  
newPerson(Nm, Born, Sx, Hm) => $person(Nm, Born, Sx, Hm).
```

The `::=` rule defines a new algebraic data type, a data type with only data constructors.

The `<~` rule defines an interface type - it indicates what properties are characteristic of a person and also gives type constraints on these properties. It documents that age is a functional property with an integer value, that lives is a unary relation over strings, and that dayOfBirth is a functional property with a value that is an object of type day.

The `$=` type rule indicates that there is also a theory label, with the functor person, for a theory that defines the characteristic properties of the person type - implements the person interface - in terms of four given parameters of types string, day , Sex, and string.

## Conflict with Google

In November 2009, Google released a similarly named Go programming language (with no exclamation point). McCabe asked Google to change the name of their language as he was concerned they were "steam-rolling over us". The issue received attention among technology news websites, with some of them characterizing Go! as "obscure". The issue thread opened on the subject was closed by a Google developer on 12 October 2010 with the custom status "Unfortunate" and with the following comment: "there are many computing products and services named Go. In the 11 months since our release, there has been minimal confusion of the two languages.

***

## Sources

[Go! programming language on Wikipedia](https://en.wikipedia.org/wiki/Go!_(programming_language))

I need more sources and better sources for this article. This article is also a stub, and needs to be expanded and rewritten in some parts.

***

## Article info

**Written on:** `2021 Saturday, October 2nd at 5:20 pm`

**Last revised on:** `2021 Saturday, October 2nd at 5:20 pm`

**File format** `Markdown document (*.md *.mkd *.markdown)`

**Line count (including blank lines and compiler line):** `89`

**Article version:** `1 (2021 Saturday, October 2nd at 5:20 pm)`

***

<!-- Tools

Quick copy and paste

https://github.com/seanpm2001/Degoogle-your-life/wiki/

!-->
