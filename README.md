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

## Syntax

<table>
  <thead>
    <tr>
      <th></th>
      <th>Ruby</th>
      <th>JavaScript</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Statements / Expressions</td>
      <td>Like Lisp Ruby is expression oriented, i.e.
      everything returns a value including
      language primitives like <code>if</code> and
      <code>case</code>.</td>
      <td>Like C, Java and Perl JavaScript makes a
      distinction between language statments like
      <code>if</code> and <code>switch</code> and
      expressions like <code>2 + 3</code>.</td>
    </tr>
    <tr>
      <td>Conditionals</td>
      <td><pre class="code ruby">
      if x < 0
        puts 'Negative'
      elsif x > 0
        puts 'Positive'
      else
        puts 'Zero'
      end
      </pre></td>
      <td><pre class="code javascript">
      if (x < 0) {
          console.log('Negative');
      }
      else if (x > 0) {
          console.log('Positive');
      }
      else {
          console.log('Zero');
      }
    </tr>
  </tbody>
</table>

|                             | Ruby                                        | JavaScript                                    |
| --------------------------- | ------------------------------------------- | --------------------------------------------- |
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

## Operators

## Object Oriented Programming

## Functional Programming

## Imperative Programming

## Concurrent Programming

## Core Types
