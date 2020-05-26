# Ruby and JavaScript--A Comparison

## Overview

|                             | Ruby                                        | JavaScript                                    |
| --------------------------- | ------------------------------------------- | --------------------------------------------- |
| Appearance                  | 1995                                        | 1995                                          |
| Original Author             | Yukihiro Matsumoto                          | Brendan Eich                                  |
| Some Influences             | Lisp, Smalltalk, Perl, C                    | Scheme (a dialect of Lisp), Self (decends from Smalltalk), Java, Perl |
| Paradigms                   | Object-Oriented, Functional, Imperative     | Object-Oriented, Functional, Imperative       |
| Type Disipline              | Dynamic, Strong                             | Dynamic, Weak                                 |
| Type Hierarchy              | Every value is decendent from a single type `Object` or `BasicObject` after Ruby 1.9. | Similar to Java has 5 primitive types: `number`, `boolean`, `string`, `null`, `undefined`, and one extension type: `Object`. ES6 adds `symbol` and `bigint`. All other types decend from `Object`. |

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
      <td>
        <pre>
        if x < 0
          puts 'Negative'
        elsif x > 0
          puts 'Positive'
        else
          puts 'Zero'
        end
        </pre>
        Like Perl Ruby also supports conditionals
        as binary operators, e.g.:
        <pre>
        puts 'Negative' if x < 0
        </pre>
      </td>
      <td>
        <pre>
        if (x < 0) {
            console.log('Negative');
        }
        else if (x > 0) {
            console.log('Positive');
        }
        else {
            console.log('Zero');
        }
        </pre>
        Like C and Java curly braces are only
        required when the clause is associated with
        more than one statement, but this is a
        feature that requires some caution, because:
        <code>
        if (x < 0)
            console.log('Negative');
            console.log('Less than zero');
        </code>
        is not the same thing as
        <code>
        if (x < 0) {
            console.log('Negative');
            console.log('Less than zero');
        }
        </code>
      </td>
    </tr>
  </tbody>
</table>

## Operators

## Object Oriented Programming

## Functional Programming

## Imperative Programming

## Concurrent Programming

## Core Types

## References

- https://brendaneich.com/2008/04/popularity/
