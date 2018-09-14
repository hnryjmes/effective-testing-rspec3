## Effective Testing with RSpec 3
###### by Myron Marston and Ian Dees

#### Notes

Introduction

* 'effective' - tests that are more valuable than the time spent to write them

* Behavior-Driven Development

Chapter 1 - Getting Started With RSpec

* How to install RSpec and write your first spec / How to organize your specifications using describe and it / How to verify desired outcomes with expect / How to interpret test failures / How to keep your specs free of repeated setup code

* Effectiveness. Do the benefits of writing the test outweigh the costs?

* First spec: groups, examples, expectations

* "A test validates that a bit of code is working properly."

* "A spec describes the desired behavior of a bit of code."

* "An example shows how a particular API is intended to be used."

* Arrange, Act, Assert

* hooks: common setup code

* "Our recommendation is to use these code-sharing techniques where they improve maintainability, lessen noise, and increase clarity."

* Exercise 1. "We've shown you three primary ways to reduce duplication in RSpec: hooks, helper methods, and let declarations. Which way did you like best for this example? Why? Can you think of situations where the others might be a better option?" - hook and let methods are quite similar, helper methods are pretty intuitive. it would depend on the context for the test which to use. overuse of the before syntax could be risky and/or harder to maintain compared to let, which is more narrowly specified.
