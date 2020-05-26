# Ruby and JavaScript--A Comparison

## Overview

|                             | Ruby                                        | JavaScript                                    |
| --------------------------- | ------------------------------------------- | --------------------------------------------- |
| Appearance                  | 1995                                        | 1995                                          |
| Motivations                 | 
| Some Influences             | Scheme, Smalltalk, Perl                     | Scheme, Self, Java, Perl                      |
| Type Disipline              | Dynamic, Strong                             | Dynamic, Weak                                 |
| Type Hierarchy              | Every value is decendent from a single type | In contrast JavaScript, similar to Java       |
|                             | `Object` or `BasicObject` after Ruby 1.9.   | has 5 primitive types: `number`, `boolean`,   |
|                             |                                             | `string`, `null`, `undefined`, and one        |
|                             |                                             | extension type: `Object`. ES6 adds `symbol`   |
|                             |                                             | and `bigint`. All other types decend from     |
|                             |                                             | `Object`.                                     |
| Paradigms                   | Object-Oriented, Functional, Imperative     | Object-Oriented, Functional, Imperative       |
| --------------------------- | ------------------------------------------- | --------------------------------------------- |

## Syntax

|                             | Ruby                                        | JavaScript                                    |
| --------------------------- | ------------------------------------------- | --------------------------------------------- |
| Statements / Expressions    | Like Lisp Ruby is expression oriented, i.e. | Like C, Java and Perl JavaScript makes a      |
|                             | everything returns a value including        | distinction between language statments like   |
|                             | language primitives like `if` and `case`.   | `if` and `switch` and expressions like        |
|                             |                                             | `2 + 3`.                                      |
| Conditionals                | ```ruby                                     | ```javascript                                 |
|                             | if x < 0                                    | if (x < 0) {                                  |
|                             |   puts 'Negative'                           |    console.log('Negative');                   |
|                             | elsif x > 0                                 | }                                             |
|                             |   puts 'Positive'                           | else if (x > 0) {                             |
|                             | else                                        |    console.log('Positive');                   |
|                             |   puts 'Zero'                               | }                                             |
|                             | end                                         | else {                                        |
|                             | ```                                         |    console.log('Zero');                       |
|                             | Like Perl Ruby also support conditionals    | }                                             |
|                             | as binary operators, e.g.:                  | ```                                           |
|                             | ```ruby                                     | Like C and Java curly braces are only         |
|                             | puts 'Negative' if x < 0                    | required when the clause is associated with   |
|                             | ```                                         | more than one statement, but this is a        |
|                             |                                             | feature that requires some caution, because:  |
|                             |                                             | ```javascript                                 |
|                             |                                             | if (x < 0)                                    |
|                             |                                             |    console.log('Negative');                   |
|                             |                                             |    console.log('Less than zero');             |
|                             |                                             | ```                                           |
|                             |                                             | is not the same thing as                      |
|                             |                                             | ```javascript                                 |
|                             |                                             | if (x < 0) {                                  |
|                             |                                             |    console.log('Negative');                   |
|                             |                                             |    console.log('Less than zero');             |
|                             |                                             | }                                             |
|                             |                                             | ```                                           |
| --------------------------- | ------------------------------------------- | --------------------------------------------- |

## Operators

## Object Oriented Programming

## Functional Programming

## Imperative Programming

## Concurrent Programming

## Core Types
