# Ruby and JavaScript--A Comparison

## Overview

|                             | Ruby                                        | JavaScript                                    |
| --------------------------- | ------------------------------------------- | --------------------------------------------- |
| Appearance                  | 1995                                        | 1995                                          |
| Original Author             | Yukihiro Matsumoto                          | Brendan Eich                                  |
| Some Influences             | Scheme, Smalltalk, Perl, C                  | Scheme, Self (decends from Smalltalk), Java, Perl |
| Paradigms                   | Object-Oriented, Functional, Imperative     | Object-Oriented, Functional, Imperative       |
| Type Disipline              | Dynamic, Strong                             | Dynamic, Weak                                 |
| Type Hierarchy              | Every value is decendent from a single type `Object` or `BasicObject` after Ruby 1.9. | Similar to Java JavaScript has 5 primitive types: `number`, `boolean`, `string`, `null`, `undefined`, and one extension type: `Object`. ES6 adds `symbol` and `bigint`. All other types decend from `Object`. |

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
  <td>Like Scheme Ruby is expression oriented, i.e.
  everything returns a value including
  language primitives like <code>if</code> and
  <code>for</code>.</td>
  <td>Like Java and C JavaScript makes a
  distinction between language statments like
  <code>if</code> and <code>for</code> and
  expressions like <code>2 + 3</code>.</td>
</tr>
<tr>
  <td>Conditionals</td>
  <td>
<pre><code>if x < 0
  puts 'Negative'
elsif x > 0
  puts 'Positive'
else
  puts 'Zero'
end
</code></pre>
<p>Like Perl Ruby also supports conditionals
after a statement, e.g.:
<pre><code>puts 'Negative' if x < 0</code></pre>
In this case, "Negative" will be printed to the
screen if <code>x</code> is less than zero.</p>
<br>
<p>Also, <code>if</code> expressions evaluate
to the last expression that has been evaluated.
So
<pre><code>polarity = if x < 0
             'Negative'
           elsif x > 0
             'Positive'
           else
             'Zero'
           end

puts polarity</code></pre>
will yield the same results as the first example.</p>
<p>And
<pre><code>def polarity(x)
  if x < 0
    'Negative'
  elsif x > 0
    'Positive'
  else
    'Zero'
  end
end</code></pre>
is the same as
<pre><code>def polarity(x)
  if x < 0
    return 'Negative'
  elsif x > 0
    return 'Positive'
  else
    return 'Zero'
  end
end</code></pre></p>
</td>
<td>
<pre><code>if (x < 0) {
    console.log('Negative');
}
else if (x > 0) {
    console.log('Positive');
}
else {
    console.log('Zero');
}
</code></pre>
<p>Like C and Java curly braces are only
required when the clause is associated with
more than one statement, but this is a
feature that requires some caution, because:
<pre><code>if (x < 0)
    console.log('Negative');
    console.log('Less than zero');
</code></pre>
is not the same thing as
<pre><code>if (x < 0) {
    console.log('Negative');
    console.log('Less than zero');
}</code></pre></p>
</td>
</tr>
<tr>
  <td>Loops</td>
  <td></td>
  <td></td>
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
