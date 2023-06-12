# dhoang-creator Scala Guide

Whilst studying Software Engineering at college, we were not only assessed on whether the programs we created behaved as they shoyld have but also whether it adhered to a strict style guide. The aim of this style guide was to ensure that we got into the habit of writing code that was both clearly readable and properly formatted so it would be easier for others to understand. 

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
    * [Git Commits](#git-commits)
