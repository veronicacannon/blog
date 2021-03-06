---
layout: page
title: Glossary
description: This glossary is a random collection of definitions.
---
# Glossary

## WSL
Windows Subsystem Linux - a way to run Linux on your Windows 10 computer.

---

## WIMP
Windows
Icons
Menus
Pointers

---

## REPL
- read
- evaluate
- print
- loop

---

## Persistence
State preserved when program quits and restarts.

---

## Recursion
A recursive algorithm must:
1. Have a base case; an escape clause from the function
2. Change its state and move toward base case
3. Call itself recursively

---

## Algorithm
An algorithm is a step by step list of instructions to solve a problem.  
Basic instructions:
* input
* output
* math and logic
* conditional execution
* repetition

---

## Resource
A URN is similar to a person's name, while a URL is like a street address. The URN defines something's identity, while the URL provides a location. Essentially, "what" vs. "where". A URN has to be of this form <URN> ::= "urn:" <NID> ":" <NSS> where <NID> is the Namespace Identifier, and <NSS> is the Namespace Specific String.

        A URL is a URI that:
        1) identifies a resource
        2) provides the means of locating the resource by describing the way to access it
        A URL is a URI
        A URI is not necessarily a URL

## Constant Lookup Operator 
The double colon :: in Ruby is the constant lookup operator.  It's used to 
scope any constant in a module.

```ruby
module TaxRate
  BASE = 0.75

  class Calculated
    def max
      1.125
    end
  end
end
puts TaxRate::BASE
puts TaxRate::Calculated.new.max
```