# dhoang-creator Scala Guide

The aim of this style guide is to ensure that we get into the habit of writing code that is both clearly readable, properly formatted & consistent with other projects in this user profile thus ensuring that others can understand the code they are reading. 

Having read multiple engineer's code over the past few years, this is something that can certainly be worked upon as many accidentally follow readability anti-patterns.

Scala is a multi-paradigmed language which can be expressed both functionally and through object oriented design (and any degrees in between) and because of this, laying out a guide you adhere to throughout your career would ensure that there would be consistency within your work. 

This does not mean to say that once a style guide is written that it should always be adhered to without any alterations. Similar to ideas & perspectives, a style guide can change and evolve over time, it is simply that you as an individual contributor have an anchor to look back at and keep your code grounded.

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>.

## <a name='TOC'>Table of Contents</a>

1. [Document History](#history)

2. [Syntactic Style](#syntactic)
    * [Naming Convention](#naming)
    * [Line Length](#linelength)
    * [Rule of 30](#rule_of_30)
    * [Spacing and Indentation](#indent)
    * [Blank Lines (Vertical Whitespace)](#blanklines)
    * [Curly Braces](#curly)
    * [Non Curly Braces in Scala 3](non_curly_braces_in_Scala_3)
    * [Long Literals](#long_literal)
    * [Documentation Style](#doc)
    * [Imports](#imports)
    * [Pattern Matching](#pattern-matching)
    * [Infix Methods](#infix)
    * [Anonymous Methods](#anonymous)

3. [Scala Language Features](#lang)
    * [Case Classes and Immutability](#case_class_immutability)
    * [apply Method](#apply_method)
    * [override Modifier](#override_modifier)
    * [Multiple Parameter Lists](#multi-param-list)
    * [Symbolic Methods (Operator Overloading)](#symbolic_methods)
    * [Type Inference](#type_inference)
    * [Return Statements](#return)
    * [Recursion and Tail Recursion](#recursion)
    * [Implicits](#implicits)
    * [Exception Handling (Try vs try)](#exception)
    * [Options](#option)
    * [Monadic Chaining](#chaining)
    * [Symbol Literals](#symbol)

4. [Java Interoperability](#java)
    * [Java Features Missing from Scala](#java-missing-features)
    * [Traits and Abstract Classes](#java-traits)
    * [Type Aliases](#java-type-alias)
    * [Default Parameter Values](#java-default-param-values)
    * [Multiple Parameter Lists](#java-multi-param-list)
    * [Varargs](#java-varargs)
    * [Implicits](#java-implicits)
    * [Companion Objects, Static Methods and Fields](#java-companion-object)

5. [Testing](#testing)
    * [Intercepting Exceptions](#testing-intercepting)

6. [Github](#github)
    * [Github Project Naming Convention](#github-project-naming-convention)
    * [Github Project ReadMEs](#github-project-readmes)
    * [Git Commits](#git-commits)

## <a name='syntactic'>Syntactic Style</a>

### <a name='naming'>Naming Convention</a>

Since we don't come from a Java background, we mostly follow Scala's standard naming conventions

- Classes, traits, and objects should follow standard Scala convention i.e. PascalCase Style.
- Packages should follow the normal Scala package naming conventions i.e. all-lowercase ASCII letters.
- Methods/functions should be named in camelCase style.

Variable Naming Convention

- Variables should be named in camelCase style, and should have self-evident/ self-explanatory names.
- One-character variable names are allowed but only in instances of mathematical operations where the variables are only being called upon in the method signature and method body.

### <a name='linelength'>Line Length</a>

- Limit lines to 100 characters (this needs to be revisited)
- Exceptions should only include URLs (although these should follow the above convention)

### <a name='rule_of_30'>Rule of 30</a>

"If an element consists of more than 30 subelements, it is highly probable that there is a serious problem" - Refactoring in Large Software Projects

In general:
- A method should contain less than 30 lines of code
- A class should contain less than 30 methods
