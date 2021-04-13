---
layout: post
title: Three things I learned from The Ruby Koans
---

Here are (at least) three things I learned from [The Ruby Koans](http://rubykoans.com/):

Strings
- Escape characters like count as a single character if double quoted ("\n") and two characters if single quoted ('\n').
- You can interpolate variables in a double quotes ("The value is #{value}").  Doesn't work with single quotes.

Regular Expressions
- Formated as [/pattern/]
- ? means optional ([/ab?/] means b is optional)
- + mean one or more
- * means zero of more
- The left most match wins
- A class within the regular expression gives options:
  - Digits:  [/[0123456789]+/] is the same as [/[0-9]+/] is the same as [/\d+/]
  - Whitespace Characters: [/\s/]
  - Words: [/[a-zA-Z0-9_]+/] is the same as [/\w+/]
  - Negate a class by adding ^ at the start ([/[^0-9]+/]).  Shortcuts negated with capital letters ([/\D+/])
- .scan creates an array using split criteria (example_string.scan(/\w+/) would split words)

Classes
- Using attr_reader and attr_accessor allow object level variables that you can call with their name

Exceptions
- Can use begin, rescue, end to provide code in case of error during main (begin) block.
- DON'T DO IT

Iteration
- .each do |i| *code* end can be replaced by .each { |i| *code* }




